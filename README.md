# pdflibrary
Traning project for download web-pages to pdf files, using python, Jenkins, docker, k8s, etc

For using python script you must install:
python3 - pip3 pdf kit
apt - wkhtmltopdf

wkhtml PROBABLY must started with virtual display:
  1) apt install xvfb
  2) ln -s
  
  


441  apt-get install xvfb
443  printf '#!/bin/bash\nxvfb-run -a --server-args="-screen 0, 1024x768x24" /usr/bin/wkhtmltopdf -q $*' > /usr/bin/wkhtmltopdf.sh
444  sudo printf '#!/bin/bash\nxvfb-run -a --server-args="-screen 0, 1024x768x24" /usr/bin/wkhtmltopdf -q $*' > /usr/bin/wkhtmltopdf.sh
446  sudo chmod a+x /usr/bin/wkhtmltopdf.sh
447  ln -s /usr/bin/wkhtmltopdf.sh /usr/local/bin/wkhtmltopdf
448  sudo ln -s /usr/bin/wkhtmltopdf.sh /usr/local/bin/wkhtmltopdf
449  wkhtmltopdf http://www.google.com output.pdf
  



nxvfb-run -a --server-args="-screen 0, 1024x768x24"
xvfb-run -a --server-args="-screen 0, 1024x768x24" /usr/bin/wkhtmltopdf http://ya.ru ya.pdf
