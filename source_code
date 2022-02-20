from tkinter import *
import winsound

root = Tk()
c = Canvas(root, width=600, height=400, )
c.create_rectangle(0, 0, 800, 400, fill="#e3c9aa")

# Constants
black = "#000000"
sharp = "#1c1c1c"
white = "#FFFFFF"

class Key():
    def __init__(self):
        self.xC = 0
        self.yC = 0
        self.w = 0
        self.h = 0
        self.out = 0
        self.clr = "$"

    def setKeyCoordinates(self, pX, pY):
        self.xC = pX
        self.yC = pY

    def setKeyWidth(self, pW):
        self.w = pW

    def setKeyHeight(self, pH):
        self.h = pH

    def setKeyColor(self, pClr):
        self.clr = pClr

    def setKeyOutline(self, pOut):
        self.out = pOut

    def drawKey(self):
        left = self.xC - self.w / 2
        right = self.xC + self.w / 2
        top = self.yC - self.h / 2
        bottom = self.yC + self.h / 2
        c.create_rectangle(left, top, right, bottom, fill=self.clr, width=self.out)

    def checkKeyClick(self, pX, pY):
        left = self.xC - self.w / 2
        right = self.xC + self.w / 2
        top = self.yC - self.h / 2
        bottom = self.yC + self.h / 2
        if left < pX < right:
            if top < pY < bottom:
                return True
            else:
                return False


class Piano():
    def __init__(self):
        self.top_bar = Key()
        self.top_bar.setKeyCoordinates(300, 80)
        self.top_bar.setKeyColor(black)
        self.top_bar.setKeyWidth(425)
        self.top_bar.setKeyHeight(30)
        self.top_bar.drawKey()
        
        self.C = Key()
        self.C.setKeyCoordinates(120, 220)
        self.C.setKeyColor(white)
        self.C.setKeyWidth(60)
        self.C.setKeyHeight(250)
        self.C.setKeyOutline(5)
        self.C.drawKey()
        
        self.D = Key()
        self.D.setKeyCoordinates(180, 220)
        self.D.setKeyColor(white)
        self.D.setKeyWidth(60)
        self.D.setKeyHeight(250)
        self.D.setKeyOutline(5)
        self.D.drawKey()
        
        self.E = Key()
        self.E.setKeyCoordinates(240, 220)
        self.E.setKeyColor(white)
        self.E.setKeyWidth(60)
        self.E.setKeyHeight(250)
        self.E.setKeyOutline(5)
        self.E.drawKey()
        
        self.F = Key()
        self.F.setKeyCoordinates(300, 220)
        self.F.setKeyColor(white)
        self.F.setKeyWidth(60)
        self.F.setKeyHeight(250)
        self.F.setKeyOutline(5)
        self.F.drawKey()
        
        self.G = Key()
        self.G.setKeyCoordinates(360, 220)
        self.G.setKeyColor(white)
        self.G.setKeyWidth(60)
        self.G.setKeyHeight(250)
        self.G.setKeyOutline(5)
        self.G.drawKey()
         
        self.A = Key()
        self.A.setKeyCoordinates(420, 220)
        self.A.setKeyColor(white)
        self.A.setKeyWidth(60)
        self.A.setKeyHeight(250)
        self.A.setKeyOutline(5)
        self.A.drawKey()
        
        self.B = Key()
        self.B.setKeyCoordinates(480, 220)
        self.B.setKeyColor(white)
        self.B.setKeyWidth(60)
        self.B.setKeyHeight(250)
        self.B.setKeyOutline(5)
        self.B.drawKey()

        self.Db = Key()
        self.Db.setKeyCoordinates(145, 170)
        self.Db.setKeyColor(sharp)
        self.Db.setKeyWidth(30)
        self.Db.setKeyHeight(200)
        self.Db.setKeyOutline(1)
        self.Db.drawKey()

        self.Eb = Key()
        self.Eb.setKeyCoordinates(215, 170)
        self.Eb.setKeyColor(sharp)
        self.Eb.setKeyWidth(30)
        self.Eb.setKeyHeight(200)
        self.Eb.setKeyOutline(1)
        self.Eb.drawKey()

        self.Gb = Key()
        self.Gb.setKeyCoordinates(325, 170)
        self.Gb.setKeyColor(sharp)
        self.Gb.setKeyWidth(30)
        self.Gb.setKeyHeight(200)
        self.Gb.setKeyOutline(1)
        self.Gb.drawKey()

        self.Ab = Key()
        self.Ab.setKeyCoordinates(395, 170)
        self.Ab.setKeyColor(sharp)
        self.Ab.setKeyWidth(30)
        self.Ab.setKeyHeight(200)
        self.Ab.setKeyOutline(1)
        self.Ab.drawKey()
        
        self.Bb = Key()
        self.Bb.setKeyCoordinates(455, 170)
        self.Bb.setKeyColor(sharp)
        self.Bb.setKeyWidth(30)
        self.Bb.setKeyHeight(200)
        self.Bb.setKeyOutline(1)
        self.Bb.drawKey()
        
    def drawPiano(self):
        self.top_bar.drawKey()
        self.C.drawKey()
        self.D.drawKey()
        self.E.drawKey()
        self.F.drawKey()
        self.G.drawKey()
        self.A.drawKey()
        self.B.drawKey()
        self.Db.drawKey()
        self.Eb.drawKey()
        self.Gb.drawKey()
        self.Ab.drawKey()
        self.Bb.drawKey()
    
    def drawNotes(self):
        c.create_text(120, 300, text="C", fill=black)
        c.create_text(180, 300, text="D", fill=black)
        c.create_text(240, 300, text="E", fill=black)
        c.create_text(300, 300, text="F", fill=black)
        c.create_text(360, 300, text="G", fill=black)
        c.create_text(420, 300, text="A", fill=black)
        c.create_text(480, 300, text="B", fill=black)
        c.create_text(145, 210, text="C#", fill=white)
        c.create_text(145, 230, text="Db", fill=white)
        c.create_text(215, 210, text="D#", fill=white)
        c.create_text(215, 230, text="Eb", fill=white)
        c.create_text(325, 210, text="F#", fill=white)
        c.create_text(325, 230, text="Gb", fill=white)
        c.create_text(395, 210, text="G#", fill=white)
        c.create_text(395, 230, text="Ab", fill=white)
        c.create_text(455, 210, text="A#", fill=white)
        c.create_text(455, 230, text="Bb", fill=white)
        
    def click(self, pX, pY):
        if self.C.checkKeyClick(pX, pY):
            print("C")
            winsound.PlaySound("note C4.wav", winsound.SND_FILENAME)
        elif self.D.checkKeyClick(pX, pY):
              print("D")
              winsound.PlaySound("note D4.wav", winsound.SND_FILENAME)
        elif self.E.checkKeyClick(pX, pY):
              print("E")
              winsound.PlaySound("note E4.wav", winsound.SND_FILENAME)
        elif self.F.checkKeyClick(pX, pY):
              print("F")
              winsound.PlaySound("note F4.wav", winsound.SND_FILENAME)
        elif self.G.checkKeyClick(pX, pY):
              print("G")
              winsound.PlaySound("note G4.wav", winsound.SND_FILENAME)
        elif self.A.checkKeyClick(pX, pY):
              print("A")
              winsound.PlaySound("note A4.wav", winsound.SND_FILENAME)
        elif self.B.checkKeyClick(pX, pY):
              print("B")
              winsound.PlaySound("note B4.wav", winsound.SND_FILENAME)
        elif self.Db.checkKeyClick(pX, pY):
              print("C#/Db")
              winsound.PlaySound("note Db4.wav", winsound.SND_FILENAME)
        elif self.Eb.checkKeyClick(pX, pY):
              print("D#/Eb")
              winsound.PlaySound("note Eb4.wav", winsound.SND_FILENAME)
        elif self.Gb.checkKeyClick(pX, pY):
              print("F#/Gb")
              winsound.PlaySound("note Gb4.wav", winsound.SND_FILENAME)
        elif self.Ab.checkKeyClick(pX, pY):
              print("G#/Ab")
              winsound.PlaySound("note Ab4.wav", winsound.SND_FILENAME)
        elif self.Bb.checkKeyClick(pX, pY):
              print("A#/Bb")
              winsound.PlaySound("note Bb4.wav", winsound.SND_FILENAME)


# ==========
# ===MAIN===
# ==========
P = Piano()
P.drawPiano()
P.drawNotes()

def mouseClick(event):
    P.click(event.x, event.y)
    
c.bind("<Button-1>", mouseClick)
c.pack()

root.mainloop()
