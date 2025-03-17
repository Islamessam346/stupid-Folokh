you need to clone this repository for the files to work properly

if you don't know how to clone the repo you may ask chat gpt for steady process 

but if for some reason you cannot just follow theses steps

Steps to Fix This:
1. Install Git LFS on the New Machine
First, you need to make sure Git LFS is installed on the machine where you are downloading the repository. To install Git LFS:

For macOS:

bash
Copy
brew install git-lfs
For Windows: Download and install Git LFS from https://git-lfs.github.com.

For Linux:

bash
Copy
sudo apt-get install git-lfs
After installing, run:

bash
Copy
git lfs install
2. Clone the Repository Again
Next, you need to clone the repository again to ensure Git LFS pulls down the large files. When you clone the repo, Git LFS will automatically fetch the actual contents of the large files.

Run the following commands in your terminal:

bash
Copy
git clone https://github.com/Islamessam346/stupid-Folokh.git
3. Verify the Files
After cloning, you should have the actual .dll and .json files, and they will have their full size (not the small pointer files).

You can check if the files are correctly downloaded by looking for the large file sizes. For example:

bash
Copy
ls -lh path/to/dll-or-json-file
This should show the full size of the files as they were intended to be in the repository.

4. Using GitHub's Web Interface for Downloading
If you want to make sure that you always have the correct files when someone else downloads the repository:

Cloning: Cloning is the recommended method of accessing a repository that uses Git LFS. If you download the repository as a ZIP file from GitHub's web interface, Git LFS files will not be downloaded properly, as you experienced.

GitHub LFS Artifacts: If someone else is downloading the repository, make sure they have Git LFS installed and they clone the repository using git clone instead of downloading the ZIP. This way, they will also pull the large files correctly.
