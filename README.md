# CoffeeKiosk System Project

## Overview

The CoffeeKiosk System project simulates a coffee shop kiosk. Users can view a menu, create orders, and see their order details in a text-based interface similar to old computers like the Apple II or Commodore 64.

## Features

- Create and manage menu items.
- Create and manage customer orders.
- Display menu and order details.
- Interactive user input to add items to orders.
- Retro-style text interface.

## Usage

### Class: Item

#### Attributes

- `private String name`
- `private double price`
- `private int index`

#### Methods

- `public Item(String name, double price)`: Constructor to create a new item.
- Getters and setters for `name`, `price`, and `index`.

### Class: Order

#### Attributes

- `private String name`
- `private boolean ready`
- `private ArrayList<Item> items`

#### Methods

- `public Order()`: Default constructor.
- `public Order(String name)`: Overloaded constructor.
- Getters and setters for `name`, `ready`, and `items`.
- `public void addItem(Item item)`: Adds an item to the order.
- `public double getOrderTotal()`: Returns the total price of the order.
- `public String getStatusMessage()`: Returns the status message of the order.
- `public void display()`: Displays the order details.

### Class: CoffeeKiosk

#### Attributes

- `private ArrayList<Item> menu`
- `private ArrayList<Order> orders`

#### Methods

- `public CoffeeKiosk()`: Constructor to initialize menu and orders.
- `public void addMenuItem(String name, double price)`: Adds a new item to the menu.
- `public void displayMenu()`: Displays all items in the menu.
- `public void newOrder()`: Creates a new order interactively.
- `public void addMenuItemByInput()`: Allows admin to add a menu item manually (Ninja Bonus).

## Expected Output

The application will create a CoffeeKiosk instance, add menu items, display the menu, and allow users to create new orders interactively. The output will show the menu, prompt the user for their name and item selections, and finally display the order details once the user is done adding items.
