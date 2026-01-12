def calculate_bill(name, units):
    """
    Calculate electricity bill based on units consumed.
    Different pricing tiers:
    - 0-100 units: 5 per unit
    - 101-300 units: 7 per unit
    - 300+ units: 10 per unit
    """
    bill_amount = 0
    
    if units <= 100:
        bill_amount = units * 5
    elif units <= 300:
        bill_amount = (100 * 5) + ((units - 100) * 7)
    else:
        bill_amount = (100 * 5) + (200 * 7) + ((units - 300) * 10)
    
    return bill_amount

def main():
    print("=" * 50)
    print("ELECTRICITY BILL GENERATOR")
    print("=" * 50)
    
    name = input("Enter customer name: ")
    
    try:
        units = float(input("Enter units consumed: "))
        
        if units < 0:
            print("Units cannot be negative!")
            return
        
        bill = calculate_bill(name, units)
        
        print("\n" + "=" * 50)
        print("BILL DETAILS")
        print("=" * 50)
        print(f"Customer Name: {name}")
        print(f"Units Consumed: {units}")
        print(f"Total Bill Amount: ${bill:.2f}")
        print("=" * 50)
        
    except ValueError:
        print("Please enter a valid number for units!")

if __name__ == "__main__":
    main()
