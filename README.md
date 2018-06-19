# Using pocketsphinx for speech recognition with Quadcoptor
Developed these files to clone into raspberri pi. (link in OptimomEngineer.wordpress.com) for details on project.

Carnegie Mellon University created this awesome application to help create a library. According to the site “CMU Sphinx is a set of speech recognition development libraries and tools that can be linked into speech-enabled applications. The libraries and sample code can be used for both research and commercial purposes; for instance, Sphinx2 can be used as a telephone-based recognizer, which can be used in a dialog system. Sphinx3 is a slower, more accurate decoder.”

 

INSTALL SPHINXBASE & POCKETSPHINX:
First, Building Sphinxbase
cd ~/

wget http://sourceforge.net/projects/cmusphinx/files/sphinxbase/5prealpha/sphinxbase-5prealpha.tar.gz

tar -zxvf ./sphinxbase-5prealpha.tar.gz

cd ./sphinxbase-5prealpha

./autogen.sh

./configure

make

make clean all

make check

sudo make install

 

Second, Building PocketSphinx
cd ~/

wget http://sourceforge.net/projects/cmusphinx/files/pocketsphinx/5prealpha/pocketsphinx-5prealpha.tar.gz

tar -zxvf pocketsphinx-5prealpha.tar.gz

cd ./pocketsphinx-5prealpha

./configure

./autogen.sh

make

make clean all

make check

sudo make install

Finall, if you want to have CMUSphinx library models and training you can also redo the same steps for this source forge site.

https://sourceforge.net/projects/cmusphinx/files/sphinxtrain/5prealpha/



