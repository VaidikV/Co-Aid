from tkinter import *

BACKGROUND_COLOR = "#B1DDC6"
FONT = ("helvetica", 10, "bold")

# ----------------------------------- TODOS -----------------------------------
# todo: messagebox when nothing is typed in username or password
# todo: Next page after login

# ----------------------------------- FUNCTIONS -----------------------------------


def login():
    fetch_username = username_entry.get()
    fetch_password = password_entry.get()

    if fetch_username == "staff" and fetch_password == "123456":
        print("login success")
    else:
        invalid_password = Label(login_screen,
                                 text="Invalid username or password",
                                 bg=BACKGROUND_COLOR,
                                 fg="red",
                                 font=("Ariel", 14, "normal"),
                                 pady=10
                                 )
        invalid_password.grid(row=5, column=0, columnspan=2)


# ----------------------------------- UI SETUP -----------------------------------


# Window
window = Tk()
window.title("Co-Aid")
window.config(padx=50, pady=50, bg=BACKGROUND_COLOR)
window.geometry("+350+70")

# Frame
login_screen = Frame(window, bg=BACKGROUND_COLOR)

# Menu

# main_menu.add_command(label="Home", command=print("home"))

# window.config(menu=menubar())

# Labels
welcome_text = Label(login_screen,
                     text="Welcome to Co-Aid",
                     bg=BACKGROUND_COLOR,
                     font=("Ariel", 30, "bold")
                     )
welcome_text.grid(row=0, column=0, columnspan=2)

login_text = Label(login_screen,
                   text="Please enter the details to log in.",
                   bg=BACKGROUND_COLOR,
                   font=("Ariel", 18, "normal"),
                   pady=30
                   )
login_text.grid(row=1, column=0, columnspan=2)

username_text = Label(login_screen,
                      text="Username:",
                      bg=BACKGROUND_COLOR,
                      font=("Ariel", 15, "normal")
                      )
username_text.grid(row=2, column=0, sticky=E)
# username_text.grid_propagate()

password_text = Label(login_screen,
                      text="Password:",
                      bg=BACKGROUND_COLOR,
                      font=("Ariel", 15, "normal"),
                      pady=10
                      )
password_text.grid(row=3, column=0, sticky=E)

# Entry
username_entry = Entry(login_screen)
username_entry.grid(row=2, column=1, sticky=EW)

password_entry = Entry(login_screen)
password_entry.grid(row=3, column=1, sticky=EW)

# Buttons
login_button = Button(login_screen,
                      text="login",
                      bg=BACKGROUND_COLOR,
                      font=("Helvetica", 13),
                      command=login, )
login_button.grid(row=4, column=0, columnspan=2)

login_screen.pack()

window.mainloop()
