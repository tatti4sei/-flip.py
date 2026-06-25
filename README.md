# 1.概要  
引数で指定した画像の左右反転画像を作成する python3で動作するプログラムです。  
# 2.ソースコード  
　 # このプログラムは python3用です。  
　 # あらかじめ pip install pillow で pillow をインストールしておきます。  
   from PIL import Image  
   import sys  
   
　 # コマンドライン引数から入力画像と出力画像のファイル名を取得  
   '''python  
   input_image = sys.argv[1]  
   output_image = sys.argv[2]  
   '''  

　 # 画像の読み込み  
   '''python  
   img = Image.open(input_image)  
   '''

　 # 画像の左右反転  
   '''python
   img_flip = img.transpose(Image.FLIP_LEFT_RIGHT)
   '''

　 # 画像の保存
  '''python
  img_flip.save(output_image)
  '''
# 3.使い方  
## 3.1 実行例  
