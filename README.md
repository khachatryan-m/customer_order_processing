# customer_order_processing
Processing a pickle file of customer orders to do some data cleaning and making it fit the required format of dataframe as part of an internship task. 

Data: a binary file with customer records
Goal: Create a dataframe with the following columns and datatypes:

customer_id: int
customer_name: str
registration_date: datetime64[ns]
is_vip: bool (True if customer_id is found in vip_customers.txt, False otherwise.)
order_id: int
order_date: datetime64[ns]
product_id: int
product_name: str
category: str (Use this conversion table: {1: 'Electronics', 2: 'Apparel', 3: 'Books', 4: 'Home Goods'}. If a category value is unmappable, default it to 'Misc'.)
unit_price: float
item_quantity: int
total_item_price: float 
total_order_value_percentage: float 

The dataframe is then sorted first by customer_id, then by order_id, and finally by product_id in ascending order.
