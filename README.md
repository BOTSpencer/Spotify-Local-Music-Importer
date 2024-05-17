## User Documentation

This Python script allows you to import your local music files (MP3) into a Spotify playlist. Here's how to use it:

1. **Spotify Authentication**
   - Create a Spotify Developer account and obtain your Client ID and Client Secret.
   - The script will prompt you to enter these credentials or read them from a `secrets.json` file.

2. **Music Directory**
   - Provide the path to the directory containing your MP3 files when prompted.

3. **Accuracy Settings**
   - Choose between "normal" or "precise" compare ratio for matching MP3 filenames with Spotify track names.
   - Decide if you want to manually double-check results with low similarity during the search. This provides more precise control over which tracks are added, but it can be a tedious process due to the numerous user interactions required.[1]
   - Precise uses a DiffLib compare ratio of >95%. This means that the found track is correct with a high chance, and the amount of false positives will be low to none.[1]

4. **Log File**
   - Opt to generate a `log.csv` file containing details about the import process.

5. **Playlist Creation**
   - Choose to create a new Spotify playlist or add tracks to an existing one.
   - If creating a new playlist, provide a name for it.

The script will then search for each MP3 file on Spotify, compare the filenames, and add matching tracks to the specified playlist. Progress updates and statistics will be displayed in the console.[1]

## Limitations
- The script is limited to importing a maximum of 9999 tracks due to Spotify's API restrictions.
- Special characters in MP3 filenames are removed during the search process.[1]

## Version
This is version 1.0 of the script, and it is still in development.