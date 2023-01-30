from tkinter import *


def planet(event):
    index=int(box1.curselection()[0])
    img = List_img[index+1]
    label_img.configure(image=img)
    label_img.image = img
    label_head.config(text=List_head[index])
    label_descr.delete("1.0", END)
    label_descr.insert(END, List_descr[index])


root = Tk()
root.title("Фотографии планет Солнечной системы от NASA")
root.geometry("500x400+500+300")
root.resizable(False,False)
root.iconbitmap('img10\icon.ico')#  иконку
root.minsize(width = 250, height=200)
root.configure(background='lightblue')# задаем цвет фона

label1 = Label(text="Название планеты", fg="blue",bg="lightblue",font="Verdana 13")
label1.place(x=30,y=25)
box1=Listbox(root,height=10,width=13,selectmode=SINGLE)
box1.place(x=25,y=50)
box1.bind('<<ListboxSelect>>', planet)
box1['font']='Verdana', 15
for i in ("Меркурий","Венера","Земля","Марс","Юпитер","Сатурн","Уран","Нептун","Плутон","Ио"):
    box1.insert(END,i)

List_img=           [PhotoImage(file="img10/pic1.png"),
                    PhotoImage(file="img10/8.png"),
                    PhotoImage(file="img10/7.png"),
                    PhotoImage(file="img10/6.png"),
                    PhotoImage(file="img10/5.png"),
                    PhotoImage(file="img10/4.png"),
                    PhotoImage(file="img10/3.png"),
                    PhotoImage(file="img10/2.png"),
                    PhotoImage(file="img10/1.png"),
                    PhotoImage(file="img10/9.png"),
                    PhotoImage(file="img10/10.png")]
label_img=Label(root,image=List_img[0])
label_img.place(x=250,y=50)


label_descr=Text(root,height=5,width=23,bg="lightblue",font="Verdana 11")
label_descr.place(x=250,y=290)

List_descr =       ["Продолжительность одних    звездных суток на Меркурии составляет 58,65 земных.",
                    "Венера - самая горячая        планета Солнечной системы.",
                    "Земля является крупшейшей по диаметру, массе и плот-   ности среди планет земной   группы.",
                    "Система каньонов превыша-ет знаменитый большой ка-   ньон в 10 раз по длине, в 7 - по ширине и в 7 - по глубине",
                    "На фото видны сложные      облака планеты, легендар-   ное Большое Красное Пятно и Малое Красное Пятно.",
                    "Сатурн является уникальной планетой, украшенной тыся-чами красивых колец.",
                    "Названа в честь греческого бога неба Урана, отца   Кро-носа.",
                    "Один год на Нептуне длится 165 земных лет.",
                    "Крупнейшая по размеру       известная карликовая          планета Солнечной системы.",
                    "Ио - спутник Юпитера,          желтоватый цвет говорит о   высоком содержании серы."]


List_head =        ["Это фото планеты Меркурий",
                    "Это фото планеты Венера",
                    "Это фото планеты Земля",
                    "Это фото планеты Марс",
                    "Это фото планеты Юпитер",
                    "Это фото планеты Сатурн",
                    "Это фото планеты Уран",
                    "Это фото планеты Нептун",
                    "Это фото планеты Плутон",
                    "Это фото планеты Ио"]
label_head=Label(root, text="", fg="blue",bg="lightblue",font="Verdana 13")
label_head.place(x=240,y=25)

label2 = Label(text="Некоторые сведения", fg="blue",bg="lightblue",font="Verdana 13")
label2.place(x=250,y=260)

root.mainloop()
