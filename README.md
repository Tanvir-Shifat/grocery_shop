class GroceryList:
    def _init_(self):
        self.items = []

    def add_item(self, item):
        """Adds an item to the shopping list."""
        self.items.append(item)
        print(f"{item} added to the shopping list.")

    def remove_item(self, item):
        """Removes an item from the shopping list."""
        try:
            self.items.remove(item)
            print(f"{item} removed from the shopping list.")
        except ValueError:
            print(f"{item} not found in the shopping list.")

    def display_list(self):
        """Displays the current shopping list."""
