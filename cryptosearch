from tkinter import*
import webbrowser  

master = Tk()
e1 = Entry(master)
Label(master, text="BTC Address").grid(row=0)
e1.grid(row=0, column=1)

def open():  
    BTC = e1.get()
    a1='https://www.blockchain.com/btc/address/%s'%BTC
    a2='https://www.walletexplorer.com/wallet/0000011bd9c73aab?from_address=%s'%BTC
    a3='https://bitcoinwhoswho.com/address/%s'%BTC
    a= 'https://www.google.com/search?q=%s'%BTC
    b= 'https://search.bitchute.com/renderer?use=bitchute-json&name=Search&login=bcadmin&key=7ea2d72b62aa4f762cc5a348ef6642b8&query=%s'%BTC
    c= 'https://twitter.com/search?q=%s'%BTC
    d='https://www.youtube.com/results?search_query=%s'%BTC
    e= 'https://www.reddit.com/search/?q=%s'%BTC
    f='https://4chansearch.com/?q=%s'%BTC
    links = [a1,a2,a3,a,b,c,d,e,f]
    
    for i in links:
        try:
            webbrowser.open_new(url=i)
        except:
            print('s***...something went wrong!')

Button(master, text='Quit', command=master.quit).grid(row=3, column=0,   sticky=W, pady=4)
Button(master, text='Open', command=open).grid(row=3, column=1, sticky=W, pady=4)

mainloop( )
