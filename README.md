def main_menu():
        Мәзір_элементтері = {
            "menu_one" : {
                "Name" : 'Mikoyan-Gurevich MiG-23',
                "Price" : '100000'
            },
        
            "menu_two" : {
                "Name" : 'Trump Mobile',
                "Price" : '499'
            },
    
            "menu_three" : {
                "Name" : 'S.T.A.L.K.E.R.: Call of Pripyat',
                "Price" : '20'
            },
        
            "menu_four" : {
                "Name" : 'Hearts of Iron 4',
                "Price" : '40'
            },
        
            "menu_five" : {
                "Name" : 'Jeff Gordons 2005 Daytona 500 Hat',
                "Price" : '1000'
            },
        
        
            "menu_six" : {
                "Name" : 'Kyle Pettys No Fear Racing',
                "Price" : '70'
            },
        
            "menu_seven" : {
                "Name" : 'Fear & Hunger 2: Termina',
                "Price" : '132611'
            },
        
            "menu_eight" : {
                "Name" : 'Terminus Decree',
                "Price" : '40000'
            }
        }
    
        print("(---☆Берёзка☆---)")
        for i, items in enumerate(Мәзір_элементтері, 1):
            item = Мәзір_элементтері[items]
            print(f"{i}. {item['Name']} - ${item['Price']}")
        
        
    #Loops forever
        while True:
    #Code for picking an item
      #Мәзір_элементтері
            choice = input("\nSelect items 1-8 or leave: ")
            if choice.isdigit() and 1 <= int(choice) <= len(Мәзір_элементтері):
                keys = list(Мәзір_элементтері.keys())
                selected_key = keys[int(choice) - 1]
                selected = Мәзір_элементтері[selected_key]
                print(f"\nCustomer selected: {selected['Name']} for ${selected['Price']}")
            
            elif choice.lower() == 'leave':

                print("Leaving...")

                break
            
            
            
            else:
                print("Select a menu item or leave...")
            
            
             

 

        

        

        

 

# Tells python to run main_menu()

main_menu()

 

 

"""

# Tells python to run main_menu() but ONLY if this is not an imported python file.

 

if __name__ == "__main__":

    main_menu()

 

# You will need to know this in the future

"""
