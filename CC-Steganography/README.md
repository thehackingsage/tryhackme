# CC Steganography | https://tryhackme.com/room/ccstego

### [Task 2] Steghide

Steghide is one of the most famous steganography tools, and for good reason. It's a classic method, hiding a message inside an image, and steghide does it effectively and efficiently. A downside of steghide is that it only works on jpgs; however, that means that if you believe there is a hidden message inside a jpg, then steghide is a probable option.

One of the greatest benefits of stegohide, is that it can encrypt data with a passphrase. Meaning that if they don't have the password then they can't extract any data.

steghide can be installed with the command ```sudo apt install steghide```

#1	What argument allows you to embed data(such as files) into other files? : ```embed```

#2	What flag let's you set the file to embed? : ```-ef```

#3	What flag allows you to set the "cover file"?(i.e  the jpg) : ```-cf```

#4	How do you set the password to use for the cover file? : ```-p```

#5	What argument allows you to extract data from files? : ```extract```

#6	How do you select the file that you want to extract data from? : ```-sf```

#7	Given the passphrase "password123", what is the hidden message in the included "jpeg1" file. : ```pinguftw```

### [Task 3] zsteg

zsteg is to png's what steghide is to jpg's. It supports various techniques to extract any and all data from png files.

Note: zsteg also supports BMP files, but it is primarily used for png's.

zsteg can be installed by using ruby with the command ```gem install zsteg```

#1	How do you specify that the least significant bit comes first : ```--lsb```

#2	What about the most significant bit? : ```--msb```

#3	How do you specify verbose mode? : ```-v```

#4	How do you extract the data from a specific payload? : ```-E```

#5	In the included file "png1" what is the hidden message? : ```nootnoot$```

#6	What about the payload used to encrypt it. : ```b1,bgr,lsb,xy```

### [Task 4] Exiftool

Exiftool is a tool that allows you to view and edit image metadata. While this in itself is not a stego tool, I would be remiss not to include at least a footnote on it as one of the most popular forms of image stego is to hide messages in the metadata.

Exiftool can be installed with sudo apt install exiftool

#1	In the included jpeg3 file, what is the document name? : ```Hello :)```

### [Task 5] Stegoveritas

Personally this is one of my favorite image stego tools. It supports just about every image file, and is able to extract all types of data from it. It is an incredibly useful tool if you don't know exactly what you're looking for, as it has a myriad of built in tests to extract any and all data.

Note: Stegoveritas has other features as well such as color correcting images

Stegoveritas can be installed by running these two commands:

```pip3 install stegoveritas```

```stegoveritas_install_deps```

#1	How do you check the file for metadata? : ```-meta```

#2	How do you check for steghide hidden information : ```-steghide```

#3	What flag allows you to extract LSB data from the image? : ```-extractLSB```

#4	In the included image jpeg2 what is the hidden message? : ```kekekekek```

### [Task 6] Spectrograms

Spectrogram stegonography is the art of hiding hidden an image inside in an audio file's spectogram. Therefore when ever dealing with audio stego it is always worth analyzing the spectrogram of the audio. To do this task we will be using [Sonic Visualizer](https://www.sonicvisualiser.org/download.html).

Note: This introduction will be done using the included wav1 file.

When you open Sonic Visualizer you should see this screen:

From there click File->Open and then select the included wav1 file and you should see a screen similar to this:

From there click Layer->Add Spectrogram and you should see this:

And that's it!

#1	What is the hidden text in the included wav2 file? : ```Google```

### [Task 7] The Final Exam

Good luck and have fun!

#1	What is key 1? : ```superkeykey```

#2	What is key 2? : ```fatality```

#3	What is key 3? : ```killshot```
