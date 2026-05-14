# CS-347-Final-Project

# How I Got S&Box to Open
Important things to know first:

If S&Box was installed from Steam prior it must be deleted from wherever the steam games are stored, this goes for both the engine and its launcher tool or this won't work. I believe this is caused by it finding what existed prior so the bootstrap will not download it, but it isn't able to access those files so it can't run as it does not have everything it needs.

You will need steam installed and to be logged into it for it to launch. It doesn't matter if its a personal or a temporary school one, it just needs steam.

If you ever get the error "Steam Not Found: We can't find Steam? Is it Running? We Need Steam!" that means it failed to connect to steam in some way.



Instructions:
1. Download the source code for S&Box from github.
2. Go to where it downloaded then go to "location"\sbox-public\engine\Sandbox.Engine\Application.cs
3. Edit line 20 of that file or whichever line is 'public static ulong AppId { get; internal set; } = 590830;' then change the number at the end to be 480 instead. This is so it can connect to steam as "spacewar", and if you do not do this before the next step it will give you the Steam Not Found error. This is still required as of when I last tested on 5/1/26.
4. Then go to "download_location"\sbox-public and run the Bootstrap.bat that's inside. It will go through and install/compile everything. If this works you will have new executibles inside of sbox-public\game to launch S&Box from after it finishes.
5. Run sbox-dev.exe to open the launcher, from there you can follow along with most online tutorials for how to use the application.



# Sources / Tutorials
https://sbox.game/dev/doc
https://github.com/Facepunch/
https://www.reddit.com/r/sandbox/comments/1sms1ex/opensource_github_vs_steam_version/?solution=4028249833bccb874028249833bccb87&js_challenge=1&token=bbbe4bf1c9a2b5160829c4be34da5861b3a99b78b1611a82dec9bc3287ec7816&jsc_orig_r=
https://www.reddit.com/r/sandbox/comments/1sm7tkp/comment/ogdx0v2/?context=3&share_id=BnkoxElBpfYvnJqVOLsac&utm_content=1&utm_medium=ios_app&utm_name=ioscss&utm_source=share&utm_term=1
https://www.reddit.com/r/Steam/comments/1hrwqn1/what_is_spacewar_in_my_library/?solution=2ba4a5fa8b97f9da2ba4a5fa8b97f9da&js_challenge=1&token=bbbe4bf1c9a2b5160829c4be34da5861daa407aa3df844c13b636c4423b7a931&jsc_orig_r=
https://www.youtube.com/watch?v=X7FxCvJphGg
https://www.youtube.com/watch?v=7ClonlOIMFE
https://www.youtube.com/watch?v=e-JS8tbNo1U&list=PLIcPBTNc7_9oFEEoHSCuPrdGQnU27yLuj&index=1
https://www.youtube.com/watch?v=5hDENSPlCts&list=PLfBadXlmJmGbkvP1ryD52Lu79ChoICKze&index=1
