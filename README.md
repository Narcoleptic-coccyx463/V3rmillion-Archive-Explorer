# 📂 V3rmillion-Archive-Explorer - Search your V3rmillion archive data quickly

[![](https://img.shields.io/badge/Download-Archive-Explorer-blue.svg)](https://github.com/Narcoleptic-coccyx463/V3rmillion-Archive-Explorer)

This application provides a simple interface to search through the archived V3rmillion forum data. It runs a local database search engine on your Windows machine, allowing you to find specific posts and threads without needing a live internet connection. The tool uses a search system designed for speed and accuracy. 

## ⚙️ System Requirements

Before you begin, ensure your computer meets these requirements:

- Operating System: Windows 10 or Windows 11.
- Processor: Intel Core i3 or better.
- Memory: 4 gigabytes of RAM.
- Storage: 10 gigabytes of free disk space to house the database files.
- Software: Docker Desktop for Windows.

## 📥 Getting Started

Follow these steps to set up the explorer on your desktop.

1. Install Docker Desktop. Visit the official Docker website to download the installer for Windows. Run the installer and follow the on-screen prompts. Restart your computer after the installation finishes.
2. Visit this page to download the software: [https://github.com/Narcoleptic-coccyx463/V3rmillion-Archive-Explorer](https://github.com/Narcoleptic-coccyx463/V3rmillion-Archive-Explorer).
3. Extract the downloaded folder to a location you can easily find, such as your Documents or Downloads folder.
4. Open the extracted folder and locate the file named Setup.bat.
5. Double-click Setup.bat to begin the installation of the database index. This process may take several minutes depending on your internet speed and disk performance. 
6. Once the terminal window closes, the installation is complete.

## 🚀 Running the Application

After your installation completes, use these steps to run the software.

1. Open your Docker Desktop application and confirm the status icon shows green.
2. Navigate back to the extracted folder in your file explorer.
3. Locate the file named Launch.bat and double-click it.
4. A small terminal window will open and remain active. Keep this window open while you use the application.
5. Open your web browser and type `http://localhost:8080` into the address bar.
6. The V3rmillion-Archive-Explorer interface will load in your browser.

## 🔍 How to Use the Search Tool

The interface displays a clean search box at the top of the page. Type the keywords, usernames, or thread dates into the box and press Enter.

- Simple Search: Type a word to find every instance of that term.
- Filtering: You can filter results by date to find posts from specific months or years.
- View Results: The engine shows a list of matching threads. Click any thread title to view the full content of the archived post.
- Navigation: Use the page numbers at the bottom of the list to browse through additional findings.

## 🛠 Troubleshooting Common Issues

If you encounter errors, check these common fixes:

- Docker Desktop not running: If the page does not load, ensure Docker Desktop is open and has finished its startup sequence.
- Database missing: If the search returns no results, ensure you ran Setup.bat successfully. The database files create a sub-folder named data; check that this folder exists and contains files.
- Port conflict: If another application uses the same port, you may see an error in the terminal. Close other server applications or background services that might occupy port 8080.
- Slow Search: Large databases require time to sort. Ensure you store the data on a solid-state drive (SSD) rather than an external hard drive for the best results.

## 🛡 Security and Privacy

This application runs locally on your machine. No data leaves your computer during searches. The program interfaces only with the local SQLite database created during setup. You do not need an account to use the service, and no tracking cookies or analytics gather data from your activity. 

## 🌐 Background Information

The V3rmillion-Archive-Explorer uses Python to manage the data layers. It utilizes SQLite FTS5 for full-text searching, which allows for fast retrieval even with millions of rows of data. The web component runs through a Docker container to ensure all necessary software dependencies remain isolated from your main Windows system files. This approach makes the archive easy to remove if you no longer require it.

To remove the program, delete the folder containing the files and open Docker Desktop to remove the associated container. This action clears the database and the search engine components from your drive.

Keywords: archive, data-parsing, docker, full-text-search, python, search-engine, sqlite, sqlite-fts5, v3rmillion, web-archive