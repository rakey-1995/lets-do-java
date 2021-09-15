# lets-do-java
package main;

import java.util.Arrays;

 abstract class item{
private String ID;
private double price;
 private int Quantity;  


    public item(){
    
    
    }
    

    public void setPrice(double price) {
        this.price = price;
    }

    public void setQuantity(int Quantity) {
        this.Quantity = Quantity;
    }

    public String getID() {
        return ID;
    }

    public double getPrice() {
        return price;
    }

    public int getQuantity() {
        return Quantity;
    }

    @Override
    public String toString() {
        return "item{" + "ID=" + ID + ", price=" + price + ", Quantity=" + Quantity + '}';
    }

 }


class Book extends item{
private String title;
private String Author;

    public Book() {
    }

    public void setTitle(String title) {
        this.title = title;
    }

    public void setAuthor(String Author) {
        this.Author = Author;
    }

    public String getTitle() {
        return title;
    }

    public String getAuthor() {
        return Author;
    }

    @Override
    public String toString() {
        return "Book{" + "title=" + title + ", Author=" + Author + '}';
    }

   

}
class Bed extends item{
 
   private String Type;
    private String color;
  private   String size;
   private String Brand;

    public Bed() {
    }

    public void setType(String Type) {
        this.Type = Type;
    }

    public void setColor(String color) {
        this.color = color;
    }

    public void setSize(String size) {
        this.size = size;
    }

    public void setBrand(String Brand) {
        this.Brand = Brand;
    }

    public String getType() {
        return Type;
    }

    public String getColor() {
        return color;
    }

    public String getSize() {
        return size;
    }

    public String getBrand() {
        return Brand;
    }

    @Override
    public String toString() {
        return "Bed{" + "Type=" + Type + ", color=" + color + ", size=" + size + ", Brand=" + Brand + '}';
    }
  
}
 class Desk extends item{
private String Type;
private String Color;
  private String Material;

    public Desk() {
    }

    public void setType(String Type) {
        this.Type = Type;
    }

    public void setColor(String Color) {
        this.Color = Color;
    }

    public void setMaterial(String Material) {
        this.Material = Material;
    }

    public String getType() {
        return Type;
    }

    public String getColor() {
        return Color;
    }

    public String getMaterial() {
        return Material;
    }

    @Override
    public String toString() {
        return "Desk{" + "Type=" + Type + ", Color=" + Color + ", Material=" + Material + '}';
    }
 
 
 
 }
class ShoppingCart{
private item[]items; 
private final int MAX_SIZE=5;
 private int itemCount;
 

 
 public boolean Additem(item[]items){
  
 if(items.length==MAX_SIZE)
     return true;
 else
     
     return false;
 }
 public boolean Removeitem(String n){
 
 
 
 
 
 }

 public void viewitem(){
 System.out.println(Arrays.toString(items));
 }
    public int getItemCount() {
        return itemCount;
    }

    @Override
    public String toString() {
        return "ShoppingCart{" + "items=" + items + ", MAX_SIZE=" + MAX_SIZE + ", itemCount=" + itemCount + '}';
    }



}
 abstract class Store{
protected int AX_PRODUCTS;
protected String StoreName;
protected int ProductCount;
protected  ShoppingCart CustomerCart;
protected item[]StoreProduct;


public void ReadProuduct(String s){

 
 
 }
public void ViewProduct(){

System.out.println(CustomerCart.toString());



}
//public item SearchByID(String i){
    
    
  
//}

}
class BookStore extends Store{

    
    public  BookStore(String a){
    
    
    
    
    }





//public boolean SearchByTitle(String s){





//}

    @Override
    public void ViewProduct() {
        super.ViewProduct(); //To change body of generated methods, choose Tools | Templates.
    }

    @Override
    public void ReadProuduct(String s) {
        super.ReadProuduct(s); //To change body of generated methods, choose Tools | Templates.
    }




}
  class FurnitureStore extends Store{
     private int bed_count;

    public FurnitureStore(String s) {
        super.StoreName=s;
        
       
    }

    @Override
    public void ViewProduct() {
        super.ViewProduct(); //To change body of generated methods, choose Tools | Templates.
    }

    @Override
    public void ReadProuduct(String s) {
        super.ReadProuduct(s); //To change body of generated methods, choose Tools | Templates.
    }

    

    
     
     
      
      
      
      
      
      
  }

























