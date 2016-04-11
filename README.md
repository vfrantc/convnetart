sudo pip3 install --upgrade https://storage.googleapis.com/tensorflow/linux/cpu/tensorflow-0.7.1-cp34-none-linux_x86_64.whl
cd ~/style
git clone  https://github.com/vfrantc/convnetart.git
cd convnetart
chmod +x models/download_models.sh
python3 main.py
