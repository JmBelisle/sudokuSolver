This is the method to use tensorflow with yolov4 Tiny to solve a sudoku sheet with a webcam.

** update 18 October 2020, I added Ali Assaf algorithm to solve the sudoku.
   it is base on Algorithm X  invented by Donald Knuth. 

1- install Tensor flow yolo4
    
    cd ~
    git clone https://github.com/pythonlessons/TensorFlow-2.x-YOLOv3
    
    N.B.  youtube videos to watch   
    https://www.youtube.com/watch?v=_4A9inxGqRM
    
    B.T.W. I'm using virtual env. Check some youtube to figure it out
    https://www.youtube.com/watch?v=GNRg2P8Vqqs&t=85s
    
2-  copy everything from ~/sudokuSolver/Tensorflow_tolov4_Tiny to TensorFlow-2.X-YOlOv3
    
    cp -y -r  ~/sudokuSolver/TensorFlow_yolov4_Tiny ~/TensorFlow-2.x-YOLOv3
    
3- copy sudokuSolver.py and Statistic.py into TensorFlow-2.x-YOLOv3


4- Download the weight from google drive or create your own by inserting picture and xml into the sudoku folder

    https://drive.google.com/file/d/1ThDDBGfbFaNh1TF-NQqq2UuWlPON9YZO/view?usp=sharing
     
    Extract the the file in the checkpoints folder 
    
    cd ~/TensorFlow-2.x-YOLOv3/checkpoints
    tar -xzf yolo4Tiny.tgz 

5- Connect a webcam into the Pi4 and run 
    
    python3 detect_sudoku.py
    
    P.S. if you installed everything using a virtual environment don't forget to enable it first


     
