# Cassette Account Password Manager

## Introduction
Cassette is a free and open-source password manager designed to help you manage your growing collection of online accounts and passwords.

Cassette does not access the internet, eliminating your concerns. It employs the proven AES256 encryption algorithm to secure your information, ensuring the safety of your account passwords. Its convenient hotkey activation method makes it easy to use.

## Development Purpose
With the increasing number of personal account passwords, finding a software solution for management has become essential. While numerous similar tools exist online and browser-built-in password managers are quite effective, security incidents involving browser password leaks are all too common. Can you truly trust third-party password management software? This prompted me to develop this open-source password manager.

This software is released under the LGPL-3 license, allowing you to compile and use it yourself. I hope everyone can finally escape the frustration of forgotten passwords.

## Build Requirements
Operating Platform: Windows 7/Windows 8.1/Windows 10/Windows 11
Programming Language: C++ MFC
Build Tool: Visual Studio 2017+

When installing Visual Studio, please select the C++ and MFC-related components.
## Compilation and Build
After downloading the repository, open `Cassette.sln` directly in `Visual Studio 2017+` to compile and build.

Note: If you are building the application yourself, it is strongly recommended that you open the `res/db.key` file and modify it to use your own database key. This key encrypts the database, protecting your data security.

	{key:"Please replace this with your own key."}

## Download the Distribution
You can download our pre-compiled binary packages [here], which include the dictionary files.

## How to Use
Notice: This software includes a vocabulary file named ``words.wl`` that is not included in this repository. While the software functions without this file, the vocabulary file significantly enhances the user experience by assisting in categorizing account-related keywords. If you require the vocabulary file, please download the software release package, which contains the vocabulary file.

1. Register and Log In
The first time you open this software, a login dialog will appear. You can register a new user (locally, without internet connection) or use the default account ``root`` (blank password). If you use root, it is recommended to change the password after logging in.
 
After logging in, enter the software's main interface.

2. Set User Hotkeys
Open the User Settings dialog from the Settings menu (also accessible from the toolbar). You now need to set a user hotkey. We recommend using Ctrl+F11 as the hotkey, though you may customize it to your preference. Simply press the desired key combination directly in the text box, then click OK.

3. Add Account Types via Hotkeys
Open the software or website where you need to record account information, such as Baidu Netdisk. Then press the [Hotkey] to bring up the Add Account Type dialog box. The automatically retrieved name and keywords may not be accurate, so you need to carefully fill in the type name and keywords. **Keywords must be as precise as possible and should not duplicate other account types.**

Note: Supports automatic detection as a website for IE, Opera, Chrome, Firefox, and Edge browsers.<br/>
If your browser is not listed in the detection records, you can manually add it via the [Database - Browser Detection Configuration] menu.

After completing the form, click “Confirm” to successfully add the account type.

4. Adding Accounts via Hotkeys
For software interfaces where account types have already been added, pressing the hotkey again will bring up the account addition dialog box. Enter your account and password, then click OK to confirm.

5. Querying Accounts via Hotkeys
On software interfaces where accounts have been added, pressing the 【Hotkey】 again will display account information for the current category.<br/>
【Right-clicking】 the corresponding account name will copy it to the clipboard with an audio cue. This facilitates inputting the account into the software.<br/>
Left-clicking the account switches to password display mode. Right-clicking copies the password to the clipboard with a distinct sound effect. This facilitates inputting the password into the software.<br/>
Left-click the green button in the top-right corner to add another account. After adding an account, you must reopen this window for it to appear.

## Open Source License
Cassette is licensed under the LGPL-3.0 (or any later version). Please refer to the [LICENSE](LICENSE) file.