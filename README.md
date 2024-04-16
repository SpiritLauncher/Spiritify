# SPIRITIFY DELAYED DUE TO THE DECRYPTION SCRIPT NOT WORKING. POSSIBLY SPOTIFY BACKEND UPDATE???


<p align="center">
    <img src="https://github.com/SpiritLauncher/Spiritify/assets/96365455/59cdd3d3-6d9b-4f8d-a369-5531fcf9f586" alt="Spiritify Logo">
</p>

# Spiritify
A Standalone Spotify Mod for Spirit City: Lofi Sessions

> [!WARNING]  
> Spiritify will **ONLY** work with _Spotify Premium Subscribers_. This is due to Spotify's Limitations.

> [!NOTE]  
> Spiritify only supports Windows, and _may or may not_ be ported for Linux and MacOS Releases.

## How to install!
1. Go to the Releases Tab and Grab the latest "Spiritify-Auto.exe" file.

2. Run the "Spiritify-Auto.exe" file as Adminstrator.
> [!NOTE]  
> If you don't want to run it as Administrator, you can bypass it by starting the executable with "-m". **This WILL cause errors.**

3. You're Done! 

## Spotify Setup
Out of the box, Spiritify won't work. You would need to create an app!
1. Go to "https://developer.spotify.com/dashboard" on your browser and log in to your Spotify account.

2. Once in, create an app.
<br>![image](https://github.com/SpiritLauncher/Spiritify/assets/96365455/6ead3c3d-f419-4d20-9692-42fb95930750)

3. Set the App Name and App Description to "Spiritify". Set the redirect URI to `http://localhost:8012/auth/callback`, and enable Web API and Web Playback SDK.
<br>![image](https://github.com/SpiritLauncher/Spiritify/assets/96365455/26b40ba7-f987-4fed-81ab-e96ae20b5fe7)

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
> If you get a warning about an invalid ClientID and Client Secret, you may need to redo step 6.<br>You may also need to install Spirit City on your C: Drive, if it's on a different Drive.

If done correctly, the Terminal will close, and Spirit City will launch "like normal".

> [!IMPORTANT]  
> The terminal will pop up if your credentials go invalid. Just re-login. **(YOU DON'T NEED TO DO STEP 7 AGAIN)**

8. A new option in "Music" called "Spiritify" will be added under "Web Music Player"!
<br>_(Don't bully on the design, it's very good 👍)_
<br>![image](https://github.com/SpiritLauncher/Spiritify/assets/96365455/fa136d29-a5f4-4fba-ac1c-1ca57325765c)

Spotify will show it's playing on Spiritify.
<br>![image](https://github.com/SpiritLauncher/Spiritify/assets/96365455/92db0865-b811-45ec-bf43-38f20f69e714)

## Uninstall Spiritify
1. Go to your Spirit City Installation, and delete "SpiritCity.exe"
<br>![image](https://github.com/SpiritLauncher/Spiritify/assets/96365455/a24c9005-8e8c-4206-abdb-4c13fbc8ff0a)
<br>![image](https://github.com/SpiritLauncher/Spiritify/assets/96365455/a0977889-2554-4294-b143-06ba6182ad65)

2. Rename "SpiritCityBackup.exe" to "SpiritCity.exe"
<br>_(If you can't launch Spirit City, you can always reinstall OR verify integrity of your files.)_

------------
## Screenshots:
Will take some when I have time.

## Roadmap
- [x] Show Title
- [x] Show Artist
- [ ] Show Album

### Controls
- [x] Play/Pause
- [x] Shuffling
- [x] Looping
- [x] Skip forward/backwards
- [ ] Volume (Current workaround, control via Mobile/Desktop Apps.)
