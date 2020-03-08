# Image To Text Converter
------------
Image to text converter using pytesseract


#Installation
------------

Please run this command to install

Python 2:
```
pip install opencv-python
```
Python 3:
```
pip3 install opencv-python
```

Python 2:
```
pip install pytesseract
```
Python 3:
```
pip3 install pytesseract
```

Then run these commands to show the text：

Python 2.x
```
python run.py

```
Python 3.x

```
python3 run.py

```

#Set your Custom Language 
ben: Bangla
eng: English

```
lang='eng+ben'

```
You have to set trinee data for your specific language from here : https://github.com/tesseract-ocr/tessdata in this path `/usr/local/share/tessdata/`

#set Configure

you have to set your configuration.

```
config='--psm 6'
```

Please see the configuration details

Page segmentation modes:

  0    Orientation and script detection (OSD) only.
  
  1    Automatic page segmentation with OSD.
  
  2    Automatic page segmentation, but no OSD, or OCR.
  
  3    Fully automatic page segmentation, but no OSD. (Default)
  
  4    Assume a single column of text of variable sizes.
  
  5    Assume a single uniform block of vertically aligned text.
  
  6    Assume a single uniform block of text.
  
  7    Treat the image as a single text line.
  
  8    Treat the image as a single word.
  
  9    Treat the image as a single word in a circle.
  
 10    Treat the image as a single character.
 
 11    Sparse text. Find as much text as possible in no particular order.
 
 12    Sparse text with OSD.
 
 13    Raw line. Treat the image as a single text line, bypassing hacks that are Tesseract-specific.
 
 


Here is a sample usage of image_to_string with multiple parameters.



```
data = pytesseract.image_to_string(thresh, lang='eng', boxes=False, \
        config='--psm 10 --oem 3 -c tessedit_char_whitelist=0123456789')

```

Hire me please email me : kamruljpi@gmail.com


