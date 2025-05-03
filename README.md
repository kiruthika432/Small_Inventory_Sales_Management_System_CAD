# Small_Inventory_Sales_Management_System_CAD
.
          Title: ShopEase
Target audience: Small business owners
           Type: B2B  
       Timeline: 2 to 3 weeks
      Team size: 1 member
Features and Workflow:
                 1, Store register
                 2, Login page
                 3, Add products (name, price, category)
                 4, Add exprie date
                 5, Add stock quantity
                 6, Low stock alert
                 7, Auto update on sales
                 8, Create and print bills
                 9, Scan barcode to add items
                 10, Show total sales
                 11, Apply discounts
                 12, Calculate tax
                 13, Daily/weekly/monthly sales reports
                 14, Display top-selling products
                 15, Add regular customer details
                 16, View purchase history
                 17, View and download invoices
                 18, Alert before product expiry
                 19, Apply discounts
                 20, Add seasonal offers
                 21, Show graphs for sales, profit, loss, stocks moved etc
                 22, Collect feedback from users

System Design:
          1, Class StoreRegister:
                  -   storeId: int
                  - storeName: String
                  - ownerName: String
                  -     email: String
                  -  password: String
.
          2, Class Login:
                  -    email: String
                  - password: String
.
          3, Class Product:
                  -     productId: int
                  -          name: String
                  -         price: double
                  -      category: String
                  -    expiryDate: String
                  - stockQuantity: int
                  -       barcode: String
                  -      discount: double
.
          4, Class Customer:
                  - customerId: int
                  -       name: String
                  -      phone: String
                  -      email: String
                  -    address: String 
.
          5, Class InvoiceItem:
                  -         product: Product ( class 3)
                  -        quantity: int
                  - discountApplied: double
                  -      finalPrice: double
.
          6, Class Invoice:
                  -   invoiceId: int
                  -    customer: Customer (class 4)
                  -       items: List<InvoiceItem>
                  - totalAmount: double
                  -   taxAmount: double
                  - finalAmount: double
                  -        date: String
.
          7, Class SalesRecord:
                  -  invoice: Invoice
                  - soldDate: String
                  -    store: Store
.
          8, Class Feedback:
                  - feedbackId: int
                  -   customer: Customer (class 4)
                  -    message: String
                  -     rating: int
.
          9, Class SalesAnalytics:
                  - topSellingProducts: List<Product>
                  -         totalSales: double
                  -        totalProfit: double 
                  -             losses: double

 ![Screenshot from 2025-05-03 14-56-46](https://github.com/user-attachments/assets/6298f4b4-f88d-42b5-879b-9b4801e89747)


                  
