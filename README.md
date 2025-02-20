# How to Use Whisper on Google Colaboratory

### I. Basic Setup
1. Search for `google colab` on Google and press Enter.
2. Select the first search result or directly click this link: [Google Colaboratory](https://colab.research.google.com/?hl=zh-tw).
    ![image](https://hackmd.io/_uploads/S1Dn4WMjC.png)
3. On the Colaboratory page, click the `File` option at the top left.
4. From the dropdown menu, select `Upload Notebook`.
    ![image](https://hackmd.io/_uploads/rkrgIWMj0.png)
5. Drag and drop `Whisper.ipynb` into the `Open a notebook` page.
    ![image](https://hackmd.io/_uploads/S11ez8ViC.png)
6. After uploading, click the `Runtime` option at the top.
7. From the dropdown, select `Change runtime type`.
    ![image](https://hackmd.io/_uploads/BytOm8Ni0.png)
8. In the pop-up window, choose `Python 3` (this should be the default).
9. Set the hardware accelerator to `T4 GPU` (default is usually CPU).
10. Click the `Save` button at the bottom left.
    ![image](https://hackmd.io/_uploads/BkZ3ELEj0.png)
11. Click the `Runtime` menu again.
12. Select `Run all` (or press `Ctrl + F9`).
    **NOTE:** It’s normal to see errors at this point since no file type or file path has been selected yet. To avoid errors, run code blocks 1 through 4 first.
    ![image](https://hackmd.io/_uploads/BktbLUNjA.png)

### II. Choose Data Type & Download Transcribed Text

#### 1. YouTube Video ➔ Text File
1. Use the dropdown menu to select the data type you want to transcribe.
2. Click the `Confirm` button.
    ![image](https://hackmd.io/_uploads/Bk8cAUEsR.png)
    - Example of selected result:
        ![image](https://hackmd.io/_uploads/HJsEePNi0.png)
3. Run code block 5 and input the `YouTube video URL` in the prompt. Press Enter and wait for the transcription.
    ![image](https://hackmd.io/_uploads/rJQl72EjR.png)
4. Run code block 6 and wait until it outputs `Your Transcript is here: YOUR_FILE_NAME.mp3.txt`.
5. Click the `Refresh` button (skip if the TXT file already appears in the right panel).
6. Right-click on `YOUR_FILE_NAME.mp3.txt`.
7. Click `Download` to get your text file.
    ![image](https://hackmd.io/_uploads/S1pimnNjR.png)
    ![image](https://hackmd.io/_uploads/rkfWpXzs0.png)

#### 2. MP4 ➔ Text File
1. Use the dropdown menu to select the data type.
2. Click the `Confirm` button.
    ![image](https://hackmd.io/_uploads/BkDCfhwjR.png)
    - Example of selected result:
        ![image](https://hackmd.io/_uploads/rkDT5U4oA.png)
3. Drag and drop `<YOUR_FILE_NAME>.mp4` into the `Files` panel.
    **NOTE:** If the panel doesn’t open automatically, click the `Files` icon on the right (orange highlight below).
4. Right-click on the file.
5. Select `Copy path`.
6. Run code block 5 and paste the `file path` into the input prompt (use `Ctrl+V`). Press Enter to start conversion.
    ![image](https://hackmd.io/_uploads/Sk6ZgiEsC.png)
7. Run code block 6 and wait for the message `Your Transcript is here: YOUR_FILE_NAME.mp3.txt`.
8. Click `Refresh` (skip if the TXT file already appears).
9. Right-click on `YOUR_FILE_NAME.mp3.txt`.
10. Click `Download` to get your text file.
    ![image](https://hackmd.io/_uploads/S1RfZiViR.png)
    ![image](https://hackmd.io/_uploads/rkfWpXzs0.png)

#### 3. MP3 ➔ Text File
1. Use the dropdown menu to select the data type.
2. Click the `Confirm` button.
    ![image](https://hackmd.io/_uploads/HJg_N2DiR.png)
    - Example of selected result:
        ![image](https://hackmd.io/_uploads/ByHyo8EjC.png)
3. Drag and drop `<YOUR_FILE_NAME>.mp3` into the `Files` panel.
    **NOTE:** If the panel doesn’t open automatically, click the `Files` icon on the right (orange highlight below).
4. Right-click on the file.
5. Select `Copy path`.
6. Run code block 5 and paste the `file path` into the input prompt (use `Ctrl+V`).
    ![image](https://hackmd.io/_uploads/rk1kEvVoR.png)
7. Run code block 6 and wait for the message `Your Transcript is here: YOUR_FILE_NAME.mp3.txt`.
8. Click `Refresh`.
    ![image](https://hackmd.io/_uploads/rk2fdDNs0.png)
9. Right-click on `YOUR_FILE_NAME.mp3.txt`.
10. Click `Download` to get your text file.
    ![image](https://hackmd.io/_uploads/Hy2PtPEsR.png)
    ![image](https://hackmd.io/_uploads/rkfWpXzs0.png)

