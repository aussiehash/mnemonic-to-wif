# mnemonic-to-wif
Converts many mnemonic seeds to WIF at once

See the example image link of operation: https://imgur.com/a/wUefg23

# INSTALLATION - Windows

* Install Python 3+, i recommend the 3.7 (already has integrated pip3) 

* Install the Python pip3 feature (if not have)

* Download the github project folder and save where you prefer. Access the directory via Command Prompt (cmd) and install the requirements.txt file libraries, use the command for greater agility: 

pip install -r requirements.txt

pip3 install ecdsa

pip3 install base58

pip3 install https://download.electrum.org/3.2.3/Electrum-3.2.3.tar.gz

pip3 install pbkdf2


* Create a .txt file named "keys_mnemonics.txt" and replace the directory sample file. Or edit the existing file with your mnemonics, 1 full sentence per line.

* You can now run the code with: python.exe mnemonic_to_wif.py

In left the Prompt with execution, in Right the commands needed to make it work in Windows, as mentioned in the text here.

# INSTALLATION - Linux - Ubuntu 16.04 LTS

* Install Python3 if you have not installed it. Command: sudo apt-get install python3

* Install pip3 if you have not installed it. Command: sudo apt-get install python3-pip

* Download the github project folder and save where you prefer. Access the directory via Terminal / Shell and install the requirements.txt file libraries, use the command for greater agility:

pip install -r requirements.txt

pip3 install ecdsa

pip3 install base58

pip3 install https://download.electrum.org/3.2.3/Electrum-3.2.3.tar.gz

pip3 install pbkdf2


* Create a .txt file named "keys_mnemonics.txt" and replace the directory sample file. Or edit the existing file with your mnemonics, 1 full sentence per line.

* You can now run the code with: python3 mnemonic_to_wif.py


# SOLVING PROBLEMS

* If get erro on install pip3 electrum, make this:

pip3 install electrum-merchant

* If the method above is not enough, make:

mkdir <yourdirname>

sudo apt-get install python3-setuptools python3-pyqt5 python3-pip

cd <yourdirname>

wget https://download.electrum.org/3.0.1/Electrum-3.0.1.tar.gz

tar -xvzf Electrum-3.0.1.tar.gz

cd Electrum-3.0.1

sudo python3 setup.py install

python3 electrum

* If you still have a library missing from your system and can not install through PIP, you can separately search the dependencies reported in Terminal / Prompt and install them manually.

* For Ubuntu, you can use the command:
sudo apt install python-base58
sudo apt install python-ecdsa
sudo apt install python-base58

# RESULTS

The code will generate 2 output files:
Addresses.txt: respective addresses generated by each mnemonic line
WIFprivatekeys.txt: Private Keys in the formed compressed WIF to each mnemonic line.

When opening the file with a text editor that allows you to count the lines, you can find each address and its respective WIF by the line number (010 Editor recommend)

#It could export everything into one text file, but this would end up with the chance to quickly import multiple WIF keys at once into one wallet. Since we would have both WIF and concatenated addresses.


If you need any support, just contact me. Reddit: https://www.reddit.com/user/genius360 Email: geniusprodigy@protonmail.com

If this helped you, please leave a tip. BTC: 1FTvHvzSNeYHZpJBvFwLy3BtNLGydzwKiM
