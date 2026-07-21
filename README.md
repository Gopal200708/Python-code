products = []
total = 0

while True:
    name = input("Enter product name (or 'stop' to finish): ").strip()

    if name.lower() == "stop":
        break

    products.append(name)

    while True:
        try:
            price = int(input("Enter price: "))
            break
        except ValueError:
            print("Please enter a valid integer price.")

    total += price

print("Total quantity:", len(products))
print("Total price:", total)

cash_received = 0

while cash_received < total:
    try:
        cash = int(input("Enter cash: "))
    except ValueError:
        print("Please enter a valid integer cash.")
        continue

    cash_received += cash

    if cash_received < total:
        print("Insufficient money. Give more:", total - cash_received)

prepare_bill = input("Prepared by: ").strip()
pmode = input("Payment mode: ").strip()

print("===================Billing Calculator====================")
print("--------------------------------------------------------")
print("NEW JANTA SUPER MARKET")
print("GSTIN: 27AAECS1234P1Z5")
print("--------------------------------------------------------")
print("shop 2/3, dhannjay Height, nile more, Nallasopara(w)")
print("--------------------------------------------------------")
print("Description")
for product in products:
    print(product)
print("--------------------------------------------------------")
print("Total quantity:", len(products))
print("Total price:", total)
print("--------------------------------------------------------")
print("Cash received:", cash_received)
print("Cash return:", cash_received - total)
print("--------------------------------------------------------")
print("Replacement within 7 days with bill")
print("Customer care: 9876543210    Email: support@newjanta.com")
print("--------------------------------------------------------")
print("Prepared by:", prepare_bill)
print("Payment mode:", pmode)
print("----------------THANK YOU. VISIT AGAIN-----------------")
print("========================================================")
