Java Console Music Player

A lightweight, console-based music player built entirely with core Java libraries. Currently, this program allows users to load and control a .wav audio file directly from their terminal using simple keyboard commands.

This is an ongoing learning project focused on mastering Java's native audio APIs (javax.sound.sampled), state management, resource handling, and user input loops.

🚀 Current Features

The application currently supports the playback of a single .wav file with the following controls:

[P] Play: Starts or resumes the audio playback.

[S] Stop: Pauses the audio.

[R] Reset: Returns the audio to the very beginning (0:00).

[Q] Quit: Closes the audio clip, terminates the scanner, and exits the application safely.

It also includes robust error handling to gracefully catch missing files, unsupported audio formats, or stream errors.

🛠️ How It Works

Under the hood, the program utilizes:

File to locate the audio file on the local machine.

AudioInputStream to read the raw audio data and translate it into a stream Java understands.

Clip to load the audio stream into the system's memory, allowing for instantaneous playback and control without manual thread management.

A Scanner wrapped in a while loop to create an interactive, continuous command-line interface.

💻 How to Run

Prerequisites

Java Development Kit (JDK) 8 or higher installed on your system.

An IDE (like IntelliJ IDEA, Eclipse, or VS Code) OR a standard terminal.

A valid .wav audio file. (Note: Java's native libraries do not support .mp3 out of the box).

Running via IDE (Recommended)

Clone or download this repository.

Open the Music_Player project folder in your preferred Java IDE.

Place a .wav file inside your project directory (e.g., inside src/ or a dedicated resources/ folder).

Update the filePath string in Main.java to point to your specific audio file.

Run the Main.java file.

Interact with the menu provided in the console output.

🗺️ Roadmap & Future Improvements

This project is actively being developed. The next major milestone is transforming this single-song player into a dynamic Media Library.

Upcoming features include:

Playlists / Libraries: Storing multiple audio files using Data Structures like ArrayList or standard Arrays.

Next & Previous Controls: Adding [N] (Next) and [B] (Back) commands to navigate through the song library.

State Management: Implementing indexing logic to track the currently playing song and seamlessly load a new AudioInputStream when the user changes tracks.

File Auto-Discovery: (Potential) Automatically scanning a designated "music" folder to populate the playlist instead of hardcoding file paths.