# basic-shopping-cart1
interface CartItem {
    name: string;
    price: number;
  }
  
const shoppingCart: CartItem[] = [];

function addItem(name: string, price: number): string {
    const newItem: CartItem = { name, price };
    shoppingCart.push(newItem);
    return `${name} has been added to the cart.`;
}

function calculateTotalCost(items: CartItem[]): number {
    return items.reduce((total, item) => total + item.price, 0);
}
  

  
