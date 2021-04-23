'''import modules'''\n
import pygame
import tkinter as tkr
'''create window'''
player=tkr.Tk()
    "\n",
    "'''edit window'''\n",
    "player.title(\"Audio Player\")\n",
    "player.geometry(\"500x500\")\n",
    "\n",
    "'''get song'''\n",
    "file = \"aa.mp3\"\n",
    "\n",
    "'''action event'''\n",
    "def play():\n",
    "    pygame.init()\n",
    "    pygame.mixer.init()\n",
    "    pygame.mixer.music.load(file)\n",
    "    pygame.mixer.music.play()\n",
    "\n",
    "def stop():\n",
    "    pygame.mixer.music.stop()\n",
    "\n",
    "'''Register buttons'''\n",
    "Button1=tkr.Button(player,width=5,height=3,text=\"PLAY\",command=play)\n",
    "Button1.pack(fill=\"x\")\n",
    "Button2=tkr.Button(player,width=5,height=3,text=\"STOP\",command=stop)\n",
    "Button2.pack(fill=\"x\")\n",
    "\n",
    "'''song name'''\n",
    "label1=tkr.LabelFrame(player,text=\"SONG NAME\")\n",
    "label1.pack(fill=\"both\",expand=\"yes\")\n",
    "contents1=tkr.Label(label1,text=file)\n",
    "contents1.pack()\n",
    "\n",
    "'''activate'''\n",
    "player.mainloop()\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": []
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 3",
   "language": "python",
   "name": "python3"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.7.3"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 2
}
