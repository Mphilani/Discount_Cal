# Discount_Cal
def calculate_discount(price, discount_percent):
    """Calculate final price after applying discount if it's 20% or higher."""
    if discount_percent >= 20:
        final_price = price - (price * (discount_percent / 100))
        return final_price
    return price  


original_price = float(input("Enter the original price of the item: "))
discount_percent = float(input("Enter the discount percentage: "))

final_price = calculate_discount(original_price, discount_percent)
print(f"Final price: ${final_price:.2f}")
