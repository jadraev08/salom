menu={
    "osh": 30000,
    "lagmon": 20000,
    "shashlik": 12000,
    "somsa": 5000,
    "choy": 5000

}

def display_menu():
    print("\n  MENYU   ")


    for nom,narx in menu.items():
        print(f"{nom} - {narx} som")

def take_order():
    while True:
         taom=input("\n ovqat nomini kiriting (stop yozilsa tugaydi)").lower()
         if taom == "stop":
            break

def calculat_total():
    jami=0
    for taom in order:
        jami +=menu[taom]
    print(f" umumiy summa {jami} som")
    return jami

display_menu()
take_order()
total=calculat_total()
