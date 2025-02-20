# 如何在 Google Colaboratory 使用 Whisper 

### I. 基本設定
1. 於 Google 搜尋列中輸入 `google colab`，並按下 Enter。
2. 選擇第一筆搜尋結果，或直接點選此連結: [Google Colaboratory](https://colab.research.google.com/?hl=zh-tw)。
    ![image](https://hackmd.io/_uploads/S1Dn4WMjC.png)
3. 進入 Colaboratory 頁面之後，點選右上`檔案` 選項。
4. 在下拉選單中，選擇`上傳筆記本`。
    ![image](https://hackmd.io/_uploads/rkrgIWMj0.png)
5. 拖曳 `Whisper.ipynb` 至 `開啟筆記本` 頁面
    ![image](https://hackmd.io/_uploads/S11ez8ViC.png)
6. 完成第五步後，點擊上方 `執行階段` 的選項
7. 在下拉選單中，選擇 `變更執行階段類型`
    ![image](https://hackmd.io/_uploads/BytOm8Ni0.png)
8. 於跳出視窗中，選擇 `Python 3` (預設應該就是 Python 3 了)
9. 將硬體加速器設定為 `T4 GPU` (預設應該是 CPU)
10. 點擊左下角的 `儲存` 按鈕
    ![image](https://hackmd.io/_uploads/BkZ3ELEj0.png)
11. 再次點擊上方 `執行階段` 選項
12. 選擇 `全部執行` (也可以直接按 `Ctrl + F9`)
    **NOTED: 後面報錯是正常的，因為沒選擇資料類型和檔案位置。**
    若不想程式報錯，可以先依序執行第 1 ~ 4 的程式區塊
    ![image](https://hackmd.io/_uploads/BktbLUNjA.png)
    

### II. 決定要提取文字的資料類型 & 下載文字檔
#### 1. YouTube 影片 &#8594; 文字檔
1. 按下拉標示並選擇要提取文字的資料類型
2. 點選`確定` 按鈕
    ![image](https://hackmd.io/_uploads/Bk8cAUEsR.png)
    - 選擇結果圖示
        ![image](https://hackmd.io/_uploads/HJsEePNi0.png)
3. 執行本程式第 5 段並於輸入框內輸入 `欲轉譯的YouTube 網址` ，按下 Enter 等待轉檔
![image](https://hackmd.io/_uploads/rJQl72EjR.png)
4. 執行第 6 段程式，等待直到它輸出 `Your Transcript is here: YOUR_FILE_NAME.mp3.txt`
5. 按下 `重新整理` 按鍵 (若右側資料夾中已存在該 TXT 檔，則可跳過此步驟~
6. 右鍵點選 `YOUR_FILE_NAME.mp3.txt`
7. 點選`下載`按鈕以取得文字檔
![image](https://hackmd.io/_uploads/S1pimnNjR.png)
![image](https://hackmd.io/_uploads/rkfWpXzs0.png)

#### 2. MP4 &#8594; 文字檔
1. 按下拉標示並選擇要提取文字的資料類型
2. 點選`確定` 按鈕
    ![image](https://hackmd.io/_uploads/BkDCfhwjR.png)
    - 選擇結果圖示
        ![image](https://hackmd.io/_uploads/rkDT5U4oA.png)
3. 拖曳 `<YOUR_FILE_NAME>.mp4` 至 `資料夾` 頁面 
    **NOTED: 若未自動開啟，可透過點選右側 `資料夾` 標示 (下圖橘色標示) 開啟**
4. 右鍵點擊該檔案名稱
5. 點選 `複製路徑`
6. 執行本程式第 5 段並於輸入框內輸入 `檔案路徑` ，按下 Enter 等待轉檔 
   (或是滑鼠選到輸入框後，按下`Ctrl+V` 就行了~
![image](https://hackmd.io/_uploads/Sk6ZgiEsC.png)
7. 執行第 6 段程式，等待直到它輸出 `Your Transcript is here: YOUR_FILE_NAME.mp3.txt`
8. 按下 `重新整理` 按鍵 (若右側資料夾中已存在該 TXT 檔，則可跳過此步驟~
9. 右鍵點選 `YOUR_FILE_NAME.mp3.txt`
10. 點選`下載`按鈕以取得文字檔
![image](https://hackmd.io/_uploads/S1RfZiViR.png)
![image](https://hackmd.io/_uploads/rkfWpXzs0.png)

#### 3. MP3 &#8594; 文字檔
1. 按下拉標示並選擇要提取文字的資料類型
2. 點選`確定` 按鈕
    ![image](https://hackmd.io/_uploads/HJg_N2DiR.png)
    - 選擇結果圖示
        ![image](https://hackmd.io/_uploads/ByHyo8EjC.png)
3. 拖曳 `<YOUR_FILE_NAME>.mp3` 至 `資料夾` 頁面 
    **NOTED: 若未自動開啟，可透過點選右側 `資料夾` 標示 (下圖橘色標示) 開啟**
4. 右鍵點擊該檔案名稱
5. 點選 `複製路徑`
6. 執行本程式第 5 段並於輸入框內輸入 `檔案路徑` (選到輸入框後，`Ctrl+V` 就行了~
![image](https://hackmd.io/_uploads/rk1kEvVoR.png)
7. 執行第 6 段程式，等待直到它輸出 `Your Transcript is here: YOUR_FILE_NAME.mp3.txt`
8. 按下 `重新整理` 按鍵
![image](https://hackmd.io/_uploads/rk2fdDNs0.png)
9. 右鍵點選 `YOUR_FILE_NAME.mp3.txt`
10. 點選`下載`按鈕以取得文字檔
![image](https://hackmd.io/_uploads/Hy2PtPEsR.png)
![image](https://hackmd.io/_uploads/rkfWpXzs0.png)

<!-- ### III. 完整程式碼
1. 第一段
    ```python
    """
    1. 下載必要套件，並引用它們
    """
    !pip install yt-dlp                     # 用來下載Youtube影片
    !pip install git+https://github.com/openai/whisper.git   # 用來下載 Whisper
    !sudo apt update && sudo apt install ffmpeg      # 用 Linux 指令下載 ffmpeg，用來將 "影片檔" 轉為 "錄音檔"
    !pip install librosa                    # 用來提取聲音的特徵

    # 引用套件
    import whisper
    import time
    import librosa
    import re
    import yt_dlp as youtube_dl
    import subprocess
    from google.colab import widgets
    import ipywidgets as widgets
    from IPython.display import display
    import os
    ```
2. 第二段
    ```python
    """
    2. 選擇想使用的聲音辨識模型，基本上 base 就夠了

      若確定音檔內容皆為英文，則可於模型名稱後加上 ".en"

      若不確定音檔所使用的語言或音檔內容不是純英文，則得移除模型名稱後的 ".en"
    """
    # model = whisper.load_model("tiny.en")
    model = whisper.load_model("base")
    # model = whisper.load_model("small.en")
    # model = whisper.load_model("medium.en")
    # model = whisper.load_model("large")
    ```
3. 第三段
    ```python=
    """
    3. 這裡是處理各資料類型的函式
    """
    def youtube_filepath():
        url = input("Enter a YouTube video URL: ")

        # Create a youtube-dl options dictionary
        ydl_opts = {
            # Specify the format as bestaudio/best
            'format': 'bestaudio/best',
            # Specify the post-processor as ffmpeg to extract audio and convert to mp3
            'postprocessors': [{
                'key': 'FFmpegExtractAudio',
                'preferredcodec': 'mp3',
                'preferredquality': '192',
            }],
            # Specify the output filename as the video title
            'outtmpl': '%(title)s.%(ext)s',
        }

        # Download the video and extract the audio
        with youtube_dl.YoutubeDL(ydl_opts) as ydl:
            ydl.download([url])

        # Get the path of the file
        file_path = ydl.prepare_filename(ydl.extract_info(url, download=False))
        file_path = file_path.replace('.webm', '.mp3')
        file_path = file_path.replace('.m4a', '.mp3')
        return file_path


    def mp4_filepath():
      file_path = input("Enter the MP4 filepath: ")
      command = "ffmpeg -i '{}' -vn -ar 44100 -ac 2 -b:a 192k '{}'".format(file_path.replace("/content/", ""), file_path.replace(".mp4", ".mp3"))
      !$command
      return file_path.replace(".mp4", ".mp3")

    ```
4. 第四段
    ```python=
    """
    4. 執行本段程式, 選擇欲轉換的資料類型, 並按下確認按鈕
    """
    file_type = None

    # Create a dropdown widget for file type selection
    file_type_dropdown = widgets.Dropdown(
        options=['YouTube Link', 'MP4', 'MP3'],
        description='資料類型: ',
    )

    # Create a button to trigger the processing
    process_button = widgets.Button(description="確定")

    # Output widget to display results
    output = widgets.Output()

    # Define a function to handle the processing
    def process_file_type(b):
        with output:
            output.clear_output()  # Clear previous outputs
            print(f"選擇的資料類型為 {file_type_dropdown.value}")  
            global file_type
            file_type = file_type_dropdown.value


    # Link the button to the processing function
    process_button.on_click(process_file_type)

    # Display the dropdown, button, and output widget
    display(file_type_dropdown, process_button, output)

    ```
5. 第五段
    ```python=
    """
    5. 輸入網址或資料連結後, 按下 Enter 以開始引用第 3 段的函式
    """
    if file_type == 'YouTube Link':
        print("User selected YouTube Link.")
        file_path = youtube_filepath()
        print(file_path)

    elif file_type == 'MP4':
        print("User selected MP4.")
        file_path = mp4_filepath()
        print(file_path)

    elif file_type == 'MP3':
        print("User selected MP3.")
        file_path = input("Enter the MP3 filepath: ")
        print(file_path)

    else:
        print("User selected YouTube Link.")
        file_path = youtube_filepath()
        print(file_path)  
    ```
6. 第六段
    ```python=
    """
    6. 此階段的程式會用 Whisper 模型開始將影音轉為文字
      txt 檔案將會被儲存於右側資料夾之中
      可以直接下載
    """

    # Get the duration
    duration = librosa.get_duration(path=file_path)
    start = time.time()
    result = model.transcribe(file_path)
    end = time.time()
    seconds = end - start

    result

    print("Video length:", duration, "seconds")
    print("Transcription time:", seconds)

    # Split result["text"]  on !,? and . , but save the punctuation
    sentences = re.split("([!?.])", result["text"])

    # Join the punctuation back to the sentences
    sentences = ["".join(i) for i in zip(sentences[0::2], sentences[1::2])]
    text = "\n\n".join(sentences)
    for s in sentences:
      print(s)

    # Save the file as .txt
    name = "".join(file_path) + ".txt"
    with open(name, "w") as f:
      f.write(text)

    print("\n\n", "-"*100, "\n\nYour transcript is here:", name)
    ``` -->
