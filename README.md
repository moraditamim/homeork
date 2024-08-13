# homeork
homeork
# # Create a class called Person with attributes name and age. Create an object of the class and print its attributes.
# class Person:
#     def __init__(self, name, age):
#         self.name = name
#         self.age = age


# person1 = Person("Yaser", 20)
# print(f"Name: {person1.name}")
# print(f"Age: {person1.age}")
# # Add a method called greet to the Person class that prints a greeting message including the person's name.
# class Person:
#     def __init__(self, name, age):
#         self.name = name
#         self.age = age

#     def greet(self):
#         print(f"Hello, my name is {self.name}.")



# person1 = Person("Yaser", 20)
# print(f"Name: {person1.name}")
# print(f"Age: {person1.age}")
# person1.greet()
# # Create a class called Car with attributes make, model, and year. Include a method to print out the car's details.
# class Car:
#     def __init__(self, make, model, year):
#         self.make = make
#         self.model = model
#         self.year = year

#     def print_details(self):
#         print(f"Car Details: {self.year} {self.model} {self.make}")


# car1 = Car("Toyota", "Camry", 2021)
# car1.print_details()
# # Create a class Circle with a method to compute the area. Initialize the class with the radius.
# import math
# class Circle:
#     def __init__(self, radius):
#         self.radius = radius# Create a base class Animal with a method speak. Create two derived classes Dog and Cat that override the speak method.
# class Animal:
#     def speak(self):
#         raise NotImplementedError("Subclass must implement abstract method.")


# class Dog(Animal):
#     def speak(self):
#         return "Woof!"


# class Cat(Animal):
#     def speak(self):
#         return "Meow!"

# dog = Dog()
# cat = Cat()

# print("Dog Says:", dog.speak())
# print("Cat Says:", cat.speak())
# # Create a base class Shape with a method area. Create derived classes Square and Triangle that implement the area method.
# class Shape:
#     def area(self):
#         raise NotImplementedError("Subclass must implement abstract method.")


# class Square(Shape):
#     def __init__(self, side_length):
#         self.side_length = side_length

#     def area(self):
#         return self.side_length ** 2


# class Triangle(Shape):
#     def __init__(self, base, height):
#         self.base = base
#         self.height = height

#     def area(self):
#         return 0.5  * self.base * self.height


# square = Square(4)
# triangle = Triangle(10, 50)

# print("Area of the square:", square.area())
# print("Area of the triangle:", triangle.area())

# # Create a class Employee with attributes name and salary. Create a derived class Manager with an additional attribute department.
# class Employee:
#     def __init__(self, name, salary):
#         self.name = name
#         self.salary = salary


# class Manager(Employee):
#     def __init__(self, name, salary, department):
#         super().__init__(name, salary)
#         self.department = department


# employee = Employee("Yaser", 50000)
# manager = Manager("Mujtaba", 80000)

# print(f"Employee: Name: {employee.name}, salary: {employee.salary}")
# print(f"Manager: Name: {manager.name}, Salary: {manager.salary}, Deparment: {manager.department} ")
# # Create a base class Vehicle with a method drive. Create derived classes Bike and Truck that override the drive method.
# class Vehicle:
#     def drive(self):
#         raise NotImplementedError("Subclass must implement abstract method")


# class Bike(Vehicle):
#     def drive(self):
#         return "Riding the bike"

# class Truck(Vehicle):
#     def __del__(self):
#         return "Driving the truck!"


# bike = Bike()
# truck = Truck

# print("Bike:", bike.drive())
# print("Truck:", truck.drive())
# # Create a base class Bird with a method fly. Create derived classes Eagle and Penguin. Override the fly method in Penguin to indicate that penguins cannot fly
# class Bird:
#     raise NotImplementedError("Subclass must implement abstract method.")



#      .   return 2 * (self.length * self.width)

# # Create a base class Bird with a method fly. Create derived classes Eagle and Penguin. Override the fly method in Penguin to indicate that penguins cannot fly
# class Bird:
#     raise NotImplementedError("Subclass must implement abstract method.")


# class Eagle(Bird):
#     def fly(self):
#         return "The eagle soars high in the sky!"


# class Penguin(Bird):
#     def fly(self):
#         return "Penguin cannot fly."


# eagle = Eagle()
# penguin = Penguin()

# print("Eagle: ", eagle.fly())
# print("Penguin: ", penguin.fly())
# # Create a class Account with private attributes balance. Provide public methods to deposit and withdraw money.
# class Account:
#     def __del__(self, initial_balance=0):
#         self.__balance = initial_balance

#     def deposit(self, amount):
#         if amount > 0:
#             self.__balance += amount
#             return f"Deposited {amount}. New balance is {self.__balance}."

#         else:
#             return "Deposit amount must be positive"

#     def withdraw(self, amount):
#         if 0 < amount <= self.__balance:
#             self.__balance -= amount
#             return f"Withdraw {amount}. New balance is  {self.__balance}"
#         elif amount > self.__balance:
#             return "Withdraw amount must be positive."

#     def get_balance(self):
#         return self.__balance
# # Create a class Book with private attributes title, author, and pages. Provide public methods to get and set these attributes.
# class Book:
#     def __init__(self, title, author, pages):
#         self.__title = title
#         self.__author = author
#         self.__pages = pages

#     def get_title(self):
#         return self.__title

#     def set_title(self, title):
#         self.__title = title

#     def get_author(self):
#         return self.__author

#     def set_author(self, author):
#         self.__author = author

#     def get_pages(self):
#         self.__pages

#     def set_pages(self, pages):
#         if pages > 0:
#             self.__pages = pages
#         else:
#             raise ValueError("Number of pages must be positive.")

# # Create a class Laptop with private attributes brand, model, and price. Provide a method to apply a discount and a method to display laptop details.
# class Laptop:
#     def __init__(self, brand, model, price):
#         self.__brand = brand
#         self.__model = model
#         self.__price = price

#     def apply_discount(self, dicount_percentage):
#         if 0 <= dicount_percentage <= 100:
#             dicount_percentage = (dicount_percentage / 100) * self.__price
#             self.__price -= dicount_percentage
#             return f"Discount of {dicount_percentage}% applied. New price is {self.__price:.2f}"
#         else:
#             return "Discount percentage must be between 0 and 100."

#     def display_details(self):
#         return f"Laptop Details:\nBrand: {self.__brand}\nModel: {self.__model}\nPrice: {self.__price:.2f}."

# # Create a class BankAccount with private attributes account_number and balance. Provide methods to deposit, withdraw, and check the balance.
# class BankAccount:
#     def __init__(self, account_number, initial_balance=0):
#         self.__account_number = account_number
#         self.__balance = initial_balance

#     def deposit(self, amount):
#         if amount > 0:
#             self.__balance += amount
#             return f"Withdraw {amount}. New balance is {self.__balance}"
#         else:
#             return "Deposit amount must be positive."

#     def withdraw(self, amount):
#         if 0 < amount <= self.__balance:
#             self.__balance -= amount
#             return f"Withdraw {amount}. New balance is {self.__balance}."
#         elif amount > self.__balance:
#             return "Insufficient balance."
#         else:
#             return "Withdrawal amount must be positive."

#     def check_balance(self):
#         return self.__balance

# class Student:
#     def _init_(self, name, grade, age):
#         self.__name = name
#         self.__grade = grade
#         self.__age = age

#     def set_name(self, name):
#         self.__name = name

#     def get_name(self):
#         return self.__name

#     def set_grade(self, grade):
#         self.__grade = grade

#     def get_grade(self):
#         return self.__grade

#     def set_age(self, age):
#         self.__age = age

#     def get_age(self):
#         return self.__age

#     def details(self):
#         return f'name of sudent is {self._name}, age {self.age} by the grade of {self._grade}'

# # Create a class Library with attributes name and books (a list of Book objects). Provide methods to add and remove books.
# class Book:
#     def __init__(self, title, author):
#         self.title = title
#         self.author = author

#     def __repr__(self):
#         return f"Book(title='{self.title}',author='{self.author}')"


# class Library:
#     def __init__(self, name):
#         self.name = name
#         self.books = []

#     def add_book(self, book):
#         self.books.append(book)
#         print(f"Add {book} to the library.")

#     def remove_book(self, book):
#         if book in self.books:
#             self.books.remove(book)
#             print(f"Removed {book} from the library.")
#         else:
#             print(f"{book} not found in the library.")

#     def __repr__(self):
#         return f"Library(name='{self.name}', books={self.books})"
# # Create a class School with attributes name and students (a list of Student objects). Provide methods to add and remove students.
# class Student:
#     def __init__(self, name):
#         self.name = name


# class School:
#     def __init__(self, name):
#         self.name = name
#         self.students = []

#     def add_student(self, student):
#         self.students.append(student)

#     def remove_student(self, student):
#         if student in self.students:
#             self.students.remove(student)
# # Create a class Company with attributes name and employees (a list of Employee objects). Provide methods to add and remove employees.
# class Employee:
#     def __init__(self, name):
#         self.name = name


# class Company:
#     def __init__(self, name):
#         self.name = name
#         self.employees = []

#     def add_employees(self, employee):
#         self.employees.append(employee)

#     def remove_employees(self, employee):
#         if employee in self.employees:
#             self.employees.remove(employee)
# # Create a class Zoo with attributes name and animals (a list of Animal objects). Provide methods to add and remove animals.
# class Animals:
#     def __init__(self, animal):
#         self.animal = animal


# class Zoo:
#     def __init__(self, animal):
#         self.animal = animal
#         self.animals = []

#     def add_animals(self, animal):
#         self.animals.append(animal)

#     def remove_animal(self, animal):
#         if animal in self.animals:
#             self.animals.remove(animal)
# # Create a class Zoo with attributes name and animals (a list of Animal objects). Provide methods to add and remove animals.
# class Animals:
#     def __init__(self, animal):
#         self.animal = animal


# class Zoo:
#     def __init__(self, animal):
#         self.animal = animal
#         self.animals = []

#     def add_animals(self, animal):
#         self.animals.append(animal)

#     def remove_animal(self, animal):
#         if animal in self.animals:
#             self.animals.remove(animal)
# # Create a class FileManager with methods to read from and write to a file.
# class FileManager:
#     def __init__(self, file_path):
#         self.file_path = file_path

#     def read_file(self):
#         try:
#             with open(self.file_path, "r") as file:
#                 return file.read()
#         except Exception as e:
#             return f"error : {e}"

#     def write_file(self, content, mode="w"):
#         try:
#             with open(self.file_path, mode) as file:
#                 file.write(content)
#                 return "Write Successful"
#         except Exception as e:
#             return f"Error: {e}"
# # Create a class Log with methods to write error messages to a log file.
# class Log:
#     def __init__(self, log_file):
#         self.log_file = log_file

#     def write_error(self, message):
#         with open(self.log_file, "a") as file:
#             file.write(f"ERROR: {message}\n")

# # Create a class Config that reads configuration settings from a file and provides methods to access these settings.
# class Config:
#     def __init__(self, config_file):
#         self.config = {}
#         with open(config_file, "r") as file:
#             for line in file:
#                 key, value = line.strip().split("=")
#                 self.config[key] = value

#     def get(self, key):
#         return self.config.get(key, None)
# # Create a class Database that connects to a database and provides methods to execute queries. Handle exceptions if the connection fails.
# import sqlite3


# class Database:
#     def __init__(self, db_file):
#         try:
#             self.conn = sqlite3.connect(db_file)
#         except sqlite3.Error as e:
#             print(f"Connection failed: {e}")

#     def execute_query(self, query):
#         try:
#             cursor = self.conn.cursor()
#             cursor.execute(query)
#             self.conn.commit()
#             return cursor.fetchall()
#         except sqlite3.Error as e:
#             print(f"Query failed: {e}")
# # Create a class Report that generates a report from data in a file. Provide methods to handle exceptions if the file does not exist or cannot be read.
# class Report:
#     def __init__(self, file_path):
#         self.file_path = file_path

#     def generate(self):
#         try:
#             with open(self.file_path, "r") as file:
#                 return file.read()
#         except FileNotFoundError:
#             return "File not found"
#         except IOError:
#             return "Error reading file."

# # Create a class Ticket for a movie theater with attributes movie_name, seat_number, and price. Provide methods to display ticket details and apply discounts.
# class Ticket:
#     def __init__(self, movie, seat, price):
#         self.movie = movie
#         self.seat = seat
#         self.price = price

#     def display(self):
#         return f"Movie: {self.movie}, seat: {self.seat}, price: {self.price:.2f}"

#     def dicount(self, percent):
#         self.price *= (1 - percent / 100)
# # Create a class ShoppingCart with methods to add, remove, and display items. Each item should be an object of a class Item with attributes name and price.
# class Item:
#     def __init__(self, name, price):
#         self.name = name
#         self.price = price


# class ShoppingCart:
#     def __init__(self):
#         self.items = []

#     def add_item(self, item):
#         self.items.append(item)

#     def remove_item(self, item):
#         self.items.remove(item)

#     def display_item(self):
#         return [f"{item.name}: ${item.price:.2f}" for item in self.items]

# # Create a class Restaurant with attributes name and menu (a list of Item objects). Provide methods to add and remove items from the menu.
# class Item:
#     def __init__(self, name, price):
#         self.name = name
#         self.price = price


# class Restaurant:
#     def __init__(self, name):
#         self.name = name
#         self.menu = []

#     def add_item(self, item):
#         self.menu.append(item)

#     def remove_item(self, item):
#         self.menu.remove(item)
# # Create a class Flight with attributes flight_number, destination, and passengers (a list of Person objects). Provide methods to add and remove passengers.
# class Person:
#     def __init__(self, name):
#         self.name = name


# class Flight:
#     def __init__(self, flight_number, destination):
#         self.flight_number = flight_number
#         self.destination = destination
#         self.passengers = []

#     def add_passengers(self, person):
#         self.passengers.append(person)

#     def remove_passengers(self, person):
#         self.passengers.remove(person)
# # Create a class Hotel with attributes name and rooms (a list of Room objects). Each Room should have attributes room_number and is_occupied. Provide methods to book and check-out rooms.
# class Room:
#     def __init__(self, room_number):
#         self.room_number = room_number
#         self.is_occupied = False


# class Hotel:
#     def __init__(self, name):
#         self.name = name
#         self.rooms = []

#     def book_room(self, room):
#         if not room.is_occupied:
#             room.is_occupied = True

#     def checkout_room(self, room):
#         if room.is_occupied:
#             room.is_occupied = False
# # Create a class CounterApp that uses tkinter to create a simple counter GUI with increment and decrement buttons.
# import tkinter as tk


# class CounterApp:
#     def __init__(self,root):
#         self.count = 0
#         self.label = tk.Label(root, text=str(self.count))
#         self.label.pack()
#         increment_button = tk.Button(root, text="Increment", command=self.increment)
#         increment_button.pack()
#         decrement_button = tk.Button(root, text="Decrement", command=self.decrement)
#         decrement_button.pack()

#     def increment(self):
#         self.count += 1
#         self.label.config(text=str(self.count))

#     def decrement(self):
#         self.count -= 1
#         self.label.config(text=str(self.count))


# root = tk.Tk()
# app = CounterApp(root)
# root.mainloop()



# import tkinter as tk
# from tkinter import messagebox

# class ToDoApp:
#     def __init__(self, master):
#         self.master = master
#         self.master.title("To-Do List")

#         # Create a frame for the listbox and scrollbar
#         self.frame = tk.Frame(self.master)
#         self.frame.pack(padx=10, pady=10)

#         # Create a listbox to display tasks
#         self.task_listbox = tk.Listbox(self.frame, width=50, height=10)
#         self.task_listbox.pack(side=tk.LEFT)

#         # Create a scrollbar for the listbox
#         self.scrollbar = tk.Scrollbar(self.frame)
#         self.scrollbar.pack(side=tk.RIGHT, fill=tk.Y)

#         # Attach the scrollbar to the listbox
#         self.task_listbox.config(yscrollcommand=self.scrollbar.set)
#         self.scrollbar.config(command=self.task_listbox.yview)

#         # Entry box for new tasks
#         self.task_entry = tk.Entry(self.master, width=52)
#         self.task_entry.pack(pady=10)

#         # Add task button
#         self.add_task_button = tk.Button(self.master, text="Add Task", command=self.add_task)
#         self.add_task_button.pack(pady=5)

#         # Remove task button
#         self.remove_task_button = tk.Button(self.master, text="Remove Selected Task", command=self.remove_task)
#         self.remove_task_button.pack(pady=5)

#     def add_task(self):
#         task = self.task_entry.get()
#         if task != "":
#             self.task_listbox.insert(tk.END, task)
#             self.task_entry.delete(0, tk.END)  # Clear the entry box
#         else:
#             messagebox.showwarning("Warning", "You must enter a task.")

#     def remove_task(self):
#         try:
#             selected_task_index = self.task_listbox.curselection()[0]
#             self.task_listbox.delete(selected_task_index)
#         except IndexError:
#             messagebox.showwarning("Warning", "You must select a task to remove.")

# if __name__ == "__main__":
#     root = tk.Tk()
#     app = ToDoApp(root)
#     root.mainloop()
    
# # Create a class CalculatorApp that uses tkinter to create a simple calculator GUI.
# import tkinter as tk

# class CalculatorApp:
#     def __init__(self, root):
#         self.root = root
#         self.root.title("Simple Calculator")

#         self.result_var = tk.StringVar()  # Variable to store the result

#         # Create the display for the calculator
#         self.result_display = tk.Entry(self.root, textvariable=self.result_var, font=("Arial", 24), justify='right')
#         self.result_display.grid(row=0, column=0, columnspan=4, padx=10, pady=10)

#         # Create buttons for the calculator
#         buttons = [
#             '7', '8', '9', '/',
#             '4', '5', '6', '*',
#             '1', '2', '3', '-',
#             'C', '0', '=', '+'
#         ]

#         row_val = 1
#         col_val = 0
#         for button in buttons:
#             if button == '=':
#                 tk.Button(self.root, text=button, command=self.calculate, height=2, width=5, font=("Arial", 18)).grid(row=row_val, column=col_val, padx=5, pady=5)
#             elif button == 'C':
#                 tk.Button(self.root, text=button, command=self.clear, height=2, width=5, font=("Arial", 18)).grid(row=row_val, column=col_val, padx=5, pady=5)
#             else:
#                 tk.Button(self.root, text=button, command=lambda b=button: self.append_to_expression(b), height=2, width=5, font=("Arial", 18)).grid(row=row_val, column=col_val, padx=5, pady=5)

#             col_val += 1
#             if col_val > 3:
#                 col_val = 0
#                 row_val += 1

#     def append_to_expression(self, value):
#         current_expression = self.result_var.get()  # Get the current expression
#         current_expression += value  # Append the new value
#         self.result_var.set(current_expression)  # Update the display

#     def calculate(self):
#         try:
#             expression = self.result_var.get()  # Get the current expression
#             result = eval(expression)  # Evaluate the expression
#             self.result_var.set(result)  # Update the display with the result
#         except Exception as e:
#             self.result_var.set("Error")  # Show error if any occurs

#     def clear(self):
#         self.result_var.set("")  # Clear the display

# if __name__ == "__main__":
#     root = tk.Tk()
#     app = CalculatorApp(root)
#     root.mainloop()
# import tkinter as tk
# from tkinter import messagebox

# class LoginApp:
#     def __init__(self, master):
#         self.master = master
#         self.master.title("Login Form")

#         # Create a frame for the form
#         self.frame = tk.Frame(self.master)
#         self.frame.pack(padx=10, pady=10)

#         # Username label and entry
#         self.username_label = tk.Label(self.frame, text="Username:")
#         self.username_label.grid(row=0, column=0, padx=5, pady=5)

#         self.username_entry = tk.Entry(self.frame)
#         self.username_entry.grid(row=0, column=1, padx=5, pady=5)

#         # Password label and entry
#         self.password_label = tk.Label(self.frame, text="Password:")
#         self.password_label.grid(row=1, column=0, padx=5, pady=5)

#         self.password_entry = tk.Entry(self.frame, show='*')  # Hide password input
#         self.password_entry.grid(row=1, column=1, padx=5, pady=5)

#         # Login button
#         self.login_button = tk.Button(self.frame, text="Login", command=self.login)
#         self.login_button.grid(row=2, columnspan=2, pady=10)

#     def login(self):
#         username = self.username_entry.get()
#         password = self.password_entry.get()

#         # Simple validation check (you can modify this logic)
#         if username == "admin" and password == "password":
#             messagebox.showinfo("Login Successful", "Welcome!")
#         else:
#             messagebox.showerror("Login Failed", "Invalid username or password.")

# if __name__ == "__main__":
#     root = tk.Tk()
#     app = LoginApp(root)
#     root.mainloop()
# import tkinter as tk
# import requests


# class WeatherApp:
#     def __init__(self, root):
#         self.root = root
#         self.root.title("Weather Information")

#         self.api_key = "your_actual_api_key"  # Replace with your OpenWeatherMap API key

#         self.cities = ["Kabul", "Herat", "Mazar", "Kandahar"]

#         # Label for dropdown menu
#         self.city_label = tk.Label(root, text="Select a City:")
#         self.city_label.pack(pady=5)

#         # Dropdown menu for city selection
#         self.city_var = tk.StringVar(value=self.cities[0])
#         self.city_menu = tk.OptionMenu(root, self.city_var, *self.cities)
#         self.city_menu.pack(pady=5)

#         # Button to fetch weather info
#         self.fetch_button = tk.Button(root, text="Get Weather", command=self.get_weather)
#         self.fetch_button.pack(pady=10)

#         # Text area to display results
#         self.result_text = tk.Text(root, height=10, width=50)
#         self.result_text.pack(pady=5)

#     def get_weather(self):
#         city = self.city_var.get()
#         url = f"http://api.openweathermap.org/data/2.5/weather?q={city}&appid={self.api_key}&units=metric"
#         response = requests.get(url)

#         if response.status_code == 200:
#             data = response.json()
#             weather_desc = data['weather'][0]['description']
#             temp = data['main']['temp']
#             feels_like = data['main']['feels_like']
#             humidity = data['main']['humidity']

#             weather_info = (f"Weather in {city}:\n"
#                             f"Description: {weather_desc}\n"
#                             f"Temperature: {temp} °C\n"
#                             f"Feels Like: {feels_like} °C\n"
#                             f"Humidity: {humidity}%\n")
#         else:
#             weather_info = f"Error: City '{city}' not found."

#         self.result_text.delete(1.0, tk.END)  # Clear the text area
#         self.result_text.insert(tk.END, weather_info)


# if __name__ == "__main__":
#     root = tk.Tk()
#     app = WeatherApp(root)
#     root.mainloop()


# # Create a class Team with attributes name and members (a list of Person objects). Provide methods to add and remove members.
# class Person:
#     def __init__(self, name):
#         self.name = name


# class Team:
#     def __init__(self, name):
#         self.name = name
#         self.members = []

#     def add_members(self, member):
#         self.members.append(member)

#     def remove_members(self, member):
#         if member in self.members:
#             self.members.remove(member)


h1
origin

