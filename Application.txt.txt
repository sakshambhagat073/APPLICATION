from tkinter import *
window = Tk()

window.title("Tickecting Application")
window.geometry('500x500')

lbl = Label(window, text="Submit Flight Data")
lbl.grid(column=1, row=0)

lbl = Label(window, text="Flight Number")
lbl.grid(column=0, row=1)
txt = Entry(window,width=20)
txt.grid(column=2, row=1)

lbl = Label(window, text="Airline Name")
lbl.grid(column=0, row=2)
txt = Entry(window,width=20)
txt.grid(column=2, row=2)

lbl = Label(window, text="Destination")
lbl.grid(column=0, row=3)
txt = Entry(window,width=20)
txt.grid(column=2, row=3)

lbl = Label(window, text="Source")
lbl.grid(column=0, row=4)
txt = Entry(window,width=20)
txt.grid(column=2, row=4)

lbl = Label(window, text="Departure")
lbl.grid(column=0, row=5)
txt = Entry(window,width=10)
txt.grid(column=2, row=5)

lbl = Label(window, text="Date")
lbl.grid(column=1, row=6)
txt = Entry(window,width=10)
txt.grid(column=2, row=6)

lbl = Label(window, text="Time")
lbl.grid(column=1, row=7)
txt = Entry(window,width=10)
txt.grid(column=2, row=7)

lbl = Label(window, text="Arrival")
lbl.grid(column=0, row=8)
txt = Entry(window,width=10)
txt.grid(column=2, row=8)

lbl = Label(window, text="Date")
lbl.grid(column=1, row=9)
txt = Entry(window,width=10)
txt.grid(column=2, row=9)


lbl = Label(window, text="Time")
lbl.grid(column=1, row=10)
txt = Entry(window,width=10)
txt.grid(column=2, row=10)

lbl = Label(window, text="Price")
lbl.grid(column=0, row=11)
txt1 = Entry(window,width=10)
txt1.grid(column=2, row=11)


def clicked():
    lbl = Label(window, text="DATA")
    lbl.grid(column=0, row=13)
    inputValue=txt1.get("1.0","END")
    print(inputValue)



btn = Button(window, text="Click Me", command=lambda: clicked())
btn.grid(column=1, row=12)



window.mainloop()
