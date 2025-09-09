# key-logger-tool
┌──(kali㉿kali)-[~]
└─$ sudo apt install python3 python3-pip python3-venv -y
[sudo] password for kali: 
python3 is already the newest version (3.13.5-1).
python3-pip is already the newest version (25.2+dfsg-1).
python3-venv is already the newest version (3.13.5-1).
The following packages were automatically installed and are no longer required:
  libbluray2  libgdata-common  libgeos3.13.1  libogdi4.1          libsframe1   libsoup-2.4-1      libtheora0     libtheoraenc1  libvpx9                python3-wheel-whl
  libgdal36   libgdata22       libhdf4-0-alt  libqt5ct-common1.8  libsigsegv2  libsoup2.4-common  libtheoradec1  libudfread0    python3-packaging-whl
Use 'sudo apt autoremove' to remove them.

Summary:
  Upgrading: 0, Installing: 0, Removing: 0, Not Upgrading: 3
                                                                                                                                                                                                                                            
┌──(kali㉿kali)-[~]
└─$ python3 -m venv venv
                                                                                                                                                                                                                                            
┌──(kali㉿kali)-[~]
└─$ source venv/bin/activate
                                                                                                                                                                                                                                            
┌──(venv)─(kali㉿kali)-[~]
└─$ pip install pynput
Requirement already satisfied: pynput in ./venv/lib/python3.13/site-packages (1.8.1)
Requirement already satisfied: six in ./venv/lib/python3.13/site-packages (from pynput) (1.17.0)
Requirement already satisfied: evdev>=1.3 in ./venv/lib/python3.13/site-packages (from pynput) (1.9.2)
Requirement already satisfied: python-xlib>=0.17 in ./venv/lib/python3.13/site-packages (from pynput) (0.33)
                                                                                                                                                                                                                                            
┌──(venv)─(kali㉿kali)-[~]
└─$ nano keylogger.py
                                                                                                                                                                                                                                            
┌──(venv)─(kali㉿kali)-[~]
└─$ python3 keylogger.py
^CTraceback (most recent call last):
  File "/home/kali/keylogger.py", line 14, in <module>
    listener.join()
    ~~~~~~~~~~~~~^^
  File "/home/kali/venv/lib/python3.13/site-packages/pynput/util/init_.py", line 295, in join
    super(AbstractListener, self).join(timeout, *args)
    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^^^^^^^^^^^^^^^^
  File "/usr/lib/python3.13/threading.py", line 1094, in join
    self._handle.join(timeout)
    ~~~~~~~~~~~~~~~~~^^^^^^^^^
KeyboardInterrupt

                                                                                                                                                                                                                                            
┌──(venv)─(kali㉿kali)-[~]
└─$ cat keylog.txt
 Key.enter  Key.ctrl  Key.alt  Key.alt tbgyvuyvbh Key.space bhouvuv Key.enter cd Key.enter 6f7 Key.backspace  Key.backspace  Key.backspace  Key.backspace  Key.backspace  Key.backspace ls Key.enter  Key.alt  Key.tab  Key.enter  Key.enter  Key.enter  Key.ctrl c Key.backspace  Key.backspace hgvdgch Key.enter jhbshveggdwvc Key.enter  Key.ctrl cc Key.backspace  Key.ctrl cy Key.shift HA Key.caps_lock ebewgyiuhrugiuahiu Key.caps_lock iuogfpogkluhihdiojui[odpuhuphgdiuhuhpus]]iojkjgnn[dihb[o]]htilidluhdiuuigiuhihg Key.enter  Key.ctrl c Key.ctrl  Key.ctrl  Key.alt tiokjbjva'n'j'fjv'nqejng[ligbli]knbgwhvknkj Key.enter yviio Key.enter  Key.ctrl c                                                                                                                                                                                                                                            
┌──(venv)─(kali㉿kali)-[~]
└─$
