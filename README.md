# Spiritify
A Standalone Spotify Mod for Spirit City: Lofi Sessions

> [!WARNING]  
> Spiritify will **ONLY** work with _Spotify Premium Subscribers_. This is due to Spotify Limitations.

> [!NOTE]  
> Spiritify only supports Windows, and _may or may not_ be ported for Linux and MacOS Releases.

## How to install!
1. Go to the Releases Tab and Grab the latest "Spiritify-Auto.zip" file.

2. Extract it, and run the "Spiritify-Auto.exe" file as Adminstrator.
> [!NOTE]  
> If you don't want to run it as Administrator, you can bypass it by starting the executable with "-m". **This WILL cause errors.**

3. You're Done! 

## Spotify Setup
Out of the box, Spiritify won't work. You would need to create an app!
1. Go to "https://developer.spotify.com/dashboard" onto your browser and log in to your Spotify account.

2. Once in, create an app.
<br>![image](https://github.com/SpiritLauncher/Spiritify/assets/96365455/6ead3c3d-f419-4d20-9692-42fb95930750)

3. Give it an App name and App description. Set the redirect URI to "http://localhost:8012", and enable Web API and Web Playback API
<br>![image](https://github.com/SpiritLauncher/Spiritify/assets/96365455/6160e6ae-1652-468a-abd0-c8324245a5b2)
> [!NOTE]  
> If you are going to use a different port, note it down. You will need to know it for later.

4. Press on settings. 
<br>![image](https://github.com/SpiritLauncher/Spiritify/assets/96365455/322fbf04-830b-42be-9b73-2bc3dc5724d2)

5. Go to your Spirit City Installation, and find the spiritify.env file.
<br>![image](https://github.com/SpiritLauncher/Spiritify/assets/96365455/a24c9005-8e8c-4206-abdb-4c13fbc8ff0a)
<br>![image](https://github.com/SpiritLauncher/Spiritify/assets/96365455/a0977889-2554-4294-b143-06ba6182ad65)

6. Open it in a text editor. You will see a file like this:
```env
PORT=8012
ClientID=""
ClientSecret=""
SpotifyUser=""
```
Fill in the ClientID and ClientSecret from the Spotify Developer Dashboard.
(e.g.
<br>![image](https://github.com/SpiritLauncher/Spiritify/assets/96365455/672f3922-b88a-481b-9be7-f358b9c5c914)
<br>For this, we will do:
```env
PORT=8012
ClientID="31a95ca027dc"
ClientSecret="f6c5eeb"
SpotifyUser=""
```
_(The above is an example. These credentials are invalid.)_
> [!NOTE]  
> If you used a different port, change "8012" to the port you set.

To obtain your Spotify User(name), you can:
- Get it from your Spotify profile URL:
<br>![image](https://github.com/SpiritLauncher/Spiritify/assets/96365455/15b46235-5441-4990-869b-d06e2e946f84)
- Get it from your Spotify Settings
<br>![image](https://github.com/SpiritLauncher/Spiritify/assets/96365455/f48893e8-ead2-47e5-8603-38c1575aebc8)

Do the same as you did with the ClientID and Client Secret, but put it in the "SpotifyUser" Area.

7. Save the file, and launch Spirit City: Lofi Sessions (Through Steam). You will see this terminal pop up.
<br>![image](https://github.com/SpiritLauncher/Spiritify/assets/96365455/dce73845-4c8b-47a9-bc02-cbf23bfacbdc)
Go onto the link, and link your Spotify Account.

> [!NOTE]  
> If you get a warning about an invalid ClinetID and Client Secret, you may need to redo step 6.<br>You may also need to install Spirit City on your C: Drive, if it's on a different Drive.

If done correctly, the Terminal will close, and Spirit City will launch "like normal".

> [!IMPORTANT]  
> The terminal will pop up if your credentials go invalid. Just re-login. **(YOU DON'T NEED TO DO STEP 7 AGAIN)**