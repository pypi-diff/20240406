# Comparing `tmp/Jetski-0.0.1.tar.gz` & `tmp/Jetski-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Jetski-0.0.1.tar", last modified: Tue Apr  2 10:31:31 2024, max compression
+gzip compressed data, was "Jetski-0.0.2.tar", last modified: Sat Apr  6 16:21:13 2024, max compression
```

## Comparing `Jetski-0.0.1.tar` & `Jetski-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 10:31:31.248427 Jetski-0.0.1/
-drwxrwxrwx   0        0        0        0 2024-04-02 10:31:31.228808 Jetski-0.0.1/Jetski/
--rw-rw-rw-   0        0        0     7698 2024-04-02 10:12:56.000000 Jetski-0.0.1/Jetski/Jetski.py
--rw-rw-rw-   0        0        0       48 2024-04-02 10:30:56.000000 Jetski-0.0.1/Jetski/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 10:31:31.247433 Jetski-0.0.1/Jetski.egg-info/
--rw-rw-rw-   0        0        0     1648 2024-04-02 10:31:31.000000 Jetski-0.0.1/Jetski.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-04-02 10:31:31.000000 Jetski-0.0.1/Jetski.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 10:31:31.000000 Jetski-0.0.1/Jetski.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-02 10:31:31.000000 Jetski-0.0.1/Jetski.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1092 2024-03-19 09:16:49.000000 Jetski-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1648 2024-04-02 10:31:31.248427 Jetski-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      648 2024-04-02 10:23:32.000000 Jetski-0.0.1/README.rst
--rw-rw-rw-   0        0        0       86 2024-04-02 10:31:31.249916 Jetski-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1341 2024-04-02 10:25:42.000000 Jetski-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 16:21:13.678070 Jetski-0.0.2/
+drwxrwxrwx   0        0        0        0 2024-04-06 16:21:13.640484 Jetski-0.0.2/Jetski/
+-rw-rw-rw-   0        0        0     7848 2024-04-06 15:40:58.000000 Jetski-0.0.2/Jetski/Jetski.py
+-rw-rw-rw-   0        0        0       48 2024-04-02 10:30:56.000000 Jetski-0.0.2/Jetski/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 16:21:13.675577 Jetski-0.0.2/Jetski.egg-info/
+-rw-rw-rw-   0        0        0     1648 2024-04-06 16:21:13.000000 Jetski-0.0.2/Jetski.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2024-04-06 16:21:13.000000 Jetski-0.0.2/Jetski.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 16:21:13.000000 Jetski-0.0.2/Jetski.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-06 16:21:13.000000 Jetski-0.0.2/Jetski.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1092 2024-03-19 09:16:49.000000 Jetski-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1648 2024-04-06 16:21:13.677564 Jetski-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      648 2024-04-06 16:02:48.000000 Jetski-0.0.2/README.rst
+-rw-rw-rw-   0        0        0       86 2024-04-06 16:21:13.680543 Jetski-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1341 2024-04-06 15:59:55.000000 Jetski-0.0.2/setup.py
```

### Comparing `Jetski-0.0.1/Jetski/Jetski.py` & `Jetski-0.0.2/Jetski/Jetski.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,71 +1,56 @@
 import datetime
 import json
-# import prettytable 
+import prettytable 
 
 class JetskiRental:
     def __init__(self,stock=0):
         self.stock = stock
 
     def displaystock(self):
-        print(f"We have currently {self.stock} jetskis available to rent.")
         return self.stock
 
     def rentJetskiOnHourlyBasis(self, n):
         if n <= 0:
             print("Number of jetskis should be positive!")
             return None
         elif n > self.stock:
             print(f"Sorry! We have currently {self.stock} jetskis available to rent.")
             return None
         else:
             now = datetime.datetime.now()
-            print(f"You have rented a {n} jetski(s) on hourly basis today at {now.hour} hours.")
-            print("You will be charged $55 for each hour per jetski.")
-            print("We hope that you enjoy our service.")
             self.stock -= n
             return now
 
     def rentJetskiOnHalfDailyBasis(self, n):
         if n <= 0:
             print("Number of jetskis should be positive!")
             return None
         elif n > self.stock:
             print(f"Sorry! We have currently {self.stock} jetskis available to rent.")
             return None
         else:
             now = datetime.datetime.now()
-            print(f"You have rented {n} jetski(s) on half daily basis today at {now.hour} hours.")
-            print("You will be charged $110 for each 4 hours per jetski.")
-            print("We hope that you enjoy our service.")
             self.stock -= n
             return now
 
     def rentJetskiOnDailyBasis(self, n):
         if n <= 0:
             print("Number of jetskis should be positive!")
             return None
         elif n > self.stock:
             print(f"Sorry! We have currently {self.stock} jetskis available to rent.")
             return None
         else:
             now = datetime.datetime.now()            
-            print(f"You have rented {n} jetski(s) on daily basis today at {now.hour} hours.")
-            print("You will be charged $165 for each 8 hrs per jetski.")
-            print("We hope that you enjoy our service.")
             self.stock -= n
             return now
 
 
     def returnJetski(self, request):
-        """
-        1. Accept a rented jetski from a customer
-        2. Replensihes the inventory (เติมของ)
-        3. Return a bill
-        """
         rentalTime, rentalBasis, numOfJetskis = request
         bill = 0
 
         if rentalTime and rentalBasis and numOfJetskis:
             self.stock += numOfJetskis
             now = datetime.datetime.now()
             rentalPeriod = now - rentalTime
@@ -77,18 +62,15 @@
                 bill = round(rentalPeriod.seconds / (3600*4)) * 110 * numOfJetskis
 
             elif rentalBasis == 3:
                 bill = round(rentalPeriod.seconds / (3600*8)) * 165 * numOfJetskis
 
             # family discount calculation
             if (3 <= numOfJetskis <= 5):
-                print("You are eligible for Family rental promotion of 20% discount")
                 bill = bill * 0.8
-            print("Thanks for returning your jetski. Hope you enjoyed our service!")
-            print(f"That would be ${bill}")
             return bill
         else:
             print("Are you sure you rented a jetski with us?")
             return None
     
     # Save
     def save_file(self, data=[], filename="JetskiInformation.json"):
@@ -104,20 +86,20 @@
         except FileNotFoundError:
             print("We don't have that file...")
 
 
 class Customer:
     def __init__(self):
         self.jetskis = 0
-        self.rentalBasis = 0                # Note: rentalBasis 1(1 hr), 2(4 hrs), 3(8 hrs) 
+        self.rentalBasis = 0
         self.rentalTime = 0
         self.bill = 0
 
     def requestJetski(self):
-        jetskis = input("How many jetskis would you like to rent?")
+        jetskis = input("How many jetskis would you like to rent? ")
 
         try:
             jetskis = int(jetskis)
         except ValueError:
             print("That's not a positive integer!")
             return -1
 
@@ -143,65 +125,91 @@
         print("1: Display informations")
         print("2: To rent jetskis")
         print("3: To return jetskis")
         print("4: Exit and Save")
         choice = input("Enter your choice (1-4): ")
         
         if choice == '1':
-            print("--------------")
+            customer = Customer()
+            myTable = prettytable.PrettyTable(["Customer", "Type", "Amount", "Start", "End", "Period(hrs)"])
+            if mydata['Customers']=={}:
+                myTable.add_row(["-","-","-","-","-","-"])
+            else:
+                for key,value in mydata['Customers'].items():
+                    list_time  = value[2]
+                    customer.rentalTime = datetime.datetime(*list_time)
+                    myTable.add_row([key, 
+                                    value[1], 
+                                    value[0],
+                                    customer.rentalTime,
+                                    "-",
+                                    "-",
+                                    ])
+            print(myTable)
             print(f"Stocks:{mydata['Stock']}")
-            for key,value in mydata['Customers'].items():
-                print(f"{key}: {value}")
-            print("--------------")
             
         elif choice == '2':
             customer = Customer()
             name = input("Enter your name: ")
-            print("--------------")
             jetskis = customer.requestJetski()
             if mydata["Stock"]>=jetskis and jetskis>=1:
                 mydata["Stock"] -= jetskis
                 rentalBasis = int(input("Choose the rentalBasis: 1(1 hr), 2(4 hrs), 3(8 hrs): "))
                 rentalTime = datetime.datetime.now()
                 date_list = list(rentalTime.timetuple())
                 del date_list[5:]
-                date_list[3] -= 2
                 mydata['Customers'][name] = [jetskis, rentalBasis, date_list]
                 shop.save_file(mydata)
-            print("--------------")
+                myTable = prettytable.PrettyTable(["Customer", "Type", "Amount", "Start", "End", "Period(hrs)", "Discount($)", "Price($)"])
+                list_time  = mydata["Customers"][name][2]
+                customer.rentalTime = datetime.datetime(*list_time)
+                myTable.add_row([name, 
+                                mydata["Customers"][name][1], 
+                                mydata["Customers"][name][0],
+                                customer.rentalTime,
+                                "-","-","-","-"
+                                ])
+                print(myTable)
             
         elif choice == '3':
             customer = Customer()
             name = input("Enter your name: ")
-            print("--------------")
             customer.jetskis = mydata["Customers"][name][0]
             customer.rentalBasis = mydata["Customers"][name][1]
             list_time  = mydata["Customers"][name][2]
             customer.rentalTime = datetime.datetime(*list_time)
             request = customer.returnJetski()
-            shop.returnJetski(request)
+            bill = shop.returnJetski(request)
             
-            '''
-            if 3<=mydata["Customers"][name][0]<=5: discount = bill
-                       
-            myTable = prettytable.PrettyTable(["Customer", "Type", "Amount", "Start", "End", "Period", "Discount", "Price"]) 
+            if 3 <= mydata["Customers"][name][0] <= 5: 
+                discount = bill/0.8 - bill
+            else:
+                discount = 0
+            
+            End = datetime.datetime.now()
+            Endlist = list(End.timetuple())
+            del Endlist[5:]
+            EndrentalTime = datetime.datetime(*Endlist)
+
+            periodTime = datetime.datetime.now()-customer.rentalTime
+            periodhour = round(periodTime.seconds / 3600)
+            myTable = prettytable.PrettyTable(["Customer", "Type", "Amount", "Start", "End", "Period(hrs)", "Discount($)", "Price($)"]) 
             myTable.add_row([name, 
                              mydata["Customers"][name][1], 
                              mydata["Customers"][name][0],
                              customer.rentalTime,
-                             datetime.datetime.now(),
-                             datetime.datetime.now()-customer.rentalTime,
+                             EndrentalTime,
+                             periodhour,
                              discount,
                              bill
                              ])
             print(myTable)
-            '''
+            
             mydata["Stock"] += mydata["Customers"][name][0]
             del mydata["Customers"][name]
             shop.save_file(mydata)
-            print("--------------")
         else:
-            break          
+            break
     
 #Test   
 if __name__ == '__main__':
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Jetski-0.0.1/Jetski.egg-info/PKG-INFO` & `Jetski-0.0.2/Jetski.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Jetski
-Version: 0.0.1
+Version: 0.0.2
 Summary: Jetski Rental System by Tarid Suwansri
 Home-page: https://github.com/TaridSuwansri/Jetski
-Download-URL: https://github.com/TaridSuwansri/Jetski/archive/v0.0.1.zip
+Download-URL: https://github.com/TaridSuwansri/Jetski/archive/v0.0.2.zip
 Author: Tarid Suwansri
 Author-email: taridsuwansri@gmail.com
 License: MIT
 Keywords: Jetski,Mathematics,Tarid,Suwansri
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Utilities
```

### Comparing `Jetski-0.0.1/LICENSE.txt` & `Jetski-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Jetski-0.0.1/PKG-INFO` & `Jetski-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Jetski
-Version: 0.0.1
+Version: 0.0.2
 Summary: Jetski Rental System by Tarid Suwansri
 Home-page: https://github.com/TaridSuwansri/Jetski
-Download-URL: https://github.com/TaridSuwansri/Jetski/archive/v0.0.1.zip
+Download-URL: https://github.com/TaridSuwansri/Jetski/archive/v0.0.2.zip
 Author: Tarid Suwansri
 Author-email: taridsuwansri@gmail.com
 License: MIT
 Keywords: Jetski,Mathematics,Tarid,Suwansri
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Utilities
```

### Comparing `Jetski-0.0.1/README.rst` & `Jetski-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `Jetski-0.0.1/setup.py` & `Jetski-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 DESCRIPTION = '\n\n'.join(LOAD_TEXT(_) for _ in [
     'README.rst'
 ])
 
 setup(
   name = 'Jetski',      
   packages = ['Jetski'], 
-  version = '0.0.1',
+  version = '0.0.2',
   license='MIT', 
   description = 'Jetski Rental System by Tarid Suwansri',
   long_description=DESCRIPTION,
   author = 'Tarid Suwansri',                 
   author_email = 'taridsuwansri@gmail.com',     
   url = 'https://github.com/TaridSuwansri/Jetski',  
-  download_url = 'https://github.com/TaridSuwansri/Jetski/archive/v0.0.1.zip',  
+  download_url = 'https://github.com/TaridSuwansri/Jetski/archive/v0.0.2.zip',  
   keywords = ['Jetski', 'Mathematics','Tarid','Suwansri'],
   classifiers=[
     'Development Status :: 3 - Alpha',     
     'Intended Audience :: Education',     
     'Topic :: Utilities',
     'License :: OSI Approved :: MIT License',   
     'Programming Language :: Python :: 3',
```

