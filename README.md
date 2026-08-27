# Offline Dlib & Face Recognition Installer for Windows

This repository is designed to help you quickly install the **dlib** and **face-recognition** libraries on Windows (64-bit) completely offline. It eliminates common installation errors such as missing CMake or Visual Studio C++ Build Tools.

It includes a pre-compiled `.conda` binary file that installs dlib natively in just a few seconds.

## 💻 System Requirements
* **OS:** Windows (64-bit)
* **Python Version:** 3.14 (running via miniconda3 / anaconda3)
* **Environment:** Miniconda Prompt or Anaconda Prompt

---

## 🚀 Installation Steps

When setting this up on a new or different computer, follow these simple steps:

### Step 1: Download the Conda Package
Download the file `dlib-20.0.1-cpu_py314hb571c67_0.conda` from this repository and save it to a local folder on your computer (e.g., directly in the `C:\` drive).

### Step 2: Open Terminal and Navigate to the Folder
Open **Miniconda Prompt** or **Anaconda Prompt** as an Administrator. Use the `cd` command to navigate to the directory where you saved the downloaded file:

```bash
cd C:\
```

### Step 3: Install Dlib Offline
Run the following command to install the dlib package locally without requiring an internet connection or compiler tools:

```bash
conda install --use-local dlib-20.0.1-cpu_py314hb571c67_0.conda
```

### Step 4: Install Face Recognition
Once the dlib installation is successfully completed, run this final command to install the face recognition module:

```bash
pip install face-recognition
```

---

## ✅ Verification
To verify that everything is installed correctly, type `python` in your terminal, press Enter, and run the following script:

```python
import dlib
import face_recognition
print("Dlib Version:", dlib.__version__)
print("Face Recognition Version:", face_recognition.__version__)
print("Setup ready to use! 🎉")
```

If the versions print successfully without any errors, your system is fully ready to run face recognition projects.

