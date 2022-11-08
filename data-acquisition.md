
pip install pytest

pip install google-search-results

from serpapi import GoogleSearch
import os, json

############################# Toilets images ########################################

image_results = []
for query in ["Toilets"]:
    params = {
        "engine": "google",   
        "q": query,                   
        "tbm": "isch",                 
        "num": "100",                     
        "ijn": 0,                         
        "api_key":("7981ea25ecca5cd1a09a815df3c8c1d9153924808ea2fe60ccd165ce1aa6680e")
    }

    search = GoogleSearch(params)         

    images_is_present = True
    while images_is_present:
        results = search.get_dict()   

        if "error" not in results:
            for image in results["images_results"]:
                if image["original"] not in image_results:
                    print(image["original"])
                    image_results.append(image["original"])
            
            params["ijn"] += 1
        else:
            images_is_present = False
            print(results["error"])

print(json.dumps(image_results, indent=2))
print(len(image_results))

############################# Bathroom Sinks images ########################################

image_results = []
for query in ["Bathroom Sinks"]:
    params = {
        "engine": "google",              
        "q": query,                       
        "tbm": "isch",                    
        "num": "100",                     
        "ijn": 0,                        
        "api_key":("7981ea25ecca5cd1a09a815df3c8c1d9153924808ea2fe60ccd165ce1aa6680e")   
    }

    search = GoogleSearch(params)        
    images_is_present = True
    while images_is_present:
        results = search.get_dict()       

        if "error" not in results:
            for image in results["images_results"]:
                if image["original"] not in image_results:
                    print(image["original"])
                    image_results.append(image["original"])
            
            params["ijn"] += 1
        else:
            images_is_present = False
            print(results["error"])

print(json.dumps(image_results, indent=2))
print(len(image_results))

############################# Showerheads images ########################################

image_results = []
for query in ["Showerheads"]:
    params = {
        "engine": "google",               
        "q": query,                      
        "tbm": "isch",                   
        "num": "100",                  
        "ijn": 0,                         
        "api_key":("7981ea25ecca5cd1a09a815df3c8c1d9153924808ea2fe60ccd165ce1aa6680e")   
    }

    search = GoogleSearch(params)      

    images_is_present = True
    while images_is_present:
        results = search.get_dict()     

        if "error" not in results:
            for image in results["images_results"]:
                if image["original"] not in image_results:
                    print(image["original"])
                    image_results.append(image["original"])
            
            # update to the next page
            params["ijn"] += 1
        else:
            images_is_present = False
            print(results["error"])

print(json.dumps(image_results, indent=2))
print(len(image_results))

############################# Bathroom Tile images ########################################

image_results = []
for query in ["Bathroom Tile"]:
    params = {
        "engine": "google",               
        "q": query,                       
        "tbm": "isch",                    
        "num": "100",                     
        "ijn": 0,                         
        "api_key":("7981ea25ecca5cd1a09a815df3c8c1d9153924808ea2fe60ccd165ce1aa6680e")   
    }

    search = GoogleSearch(params)     
    images_is_present = True
    while images_is_present:
        results = search.get_dict()   

        if "error" not in results:
            for image in results["images_results"]:
                if image["original"] not in image_results:
                    print(image["original"])
                    image_results.append(image["original"])
            
            params["ijn"] += 1
        else:
            images_is_present = False
            print(results["error"])

print(json.dumps(image_results, indent=2))
print(len(image_results))

############################# Vanities images ########################################

image_results = []
for query in ["Vanities"]:
    params = {
        "engine": "google",               
        "q": query,                       
        "tbm": "isch",                    
        "num": "100",                     
        "ijn": 0,                         
        "api_key":("7981ea25ecca5cd1a09a815df3c8c1d9153924808ea2fe60ccd165ce1aa6680e")   
    }

    search = GoogleSearch(params)         

    images_is_present = True
    while images_is_present:
        results = search.get_dict()              
        if "error" not in results:
            for image in results["images_results"]:
                if image["original"] not in image_results:
                    print(image["original"])
                    image_results.append(image["original"])
           
            params["ijn"] += 1
        else:
            images_is_present = False
            print(results["error"])

print(json.dumps(image_results, indent=2))
print(len(image_results))

############################# Faucets images ########################################

image_results = []
for query in ["Faucets"]:
    params = {
        "engine": "google",               
        "q": query,                       
        "tbm": "isch",                    
        "num": "100",                     
        "ijn": 0,                         
        "api_key":("7981ea25ecca5cd1a09a815df3c8c1d9153924808ea2fe60ccd165ce1aa6680e")   
    }

    search = GoogleSearch(params)         

    images_is_present = True
    while images_is_present:
        results = search.get_dict()       
     
        if "error" not in results:
            for image in results["images_results"]:
                if image["original"] not in image_results:
                    print(image["original"])
                    image_results.append(image["original"])
                      
            params["ijn"] += 1
        else:
            images_is_present = False
            print(results["error"])

print(json.dumps(image_results, indent=2))
print(len(image_results))

############################# Lighting images ########################################

image_results = []
for query in ["Lighting"]:
    params = {
        "engine": "google",               
        "q": query,                       
        "tbm": "isch",                    
        "num": "100",                    
        "ijn": 0,                         
        "api_key":("7981ea25ecca5cd1a09a815df3c8c1d9153924808ea2fe60ccd165ce1aa6680e")   
    }

    search = GoogleSearch(params)         

    images_is_present = True
    while images_is_present:
        results = search.get_dict()            
        if "error" not in results:
            for image in results["images_results"]:
                if image["original"] not in image_results:
                    print(image["original"])
                    image_results.append(image["original"])
                     
            params["ijn"] += 1
        else:
            images_is_present = False
            print(results["error"])

print(json.dumps(image_results, indent=2))
print(len(image_results))

############################# Cabinets & Storage images ########################################

image_results = []
for query in ["Cabinets & Storage"]:
    params = {
        "engine": "google",               
        "q": query,                       
        "tbm": "isch",                   
        "num": "100",                     
        "ijn": 0,                         
        "api_key":("7981ea25ecca5cd1a09a815df3c8c1d9153924808ea2fe60ccd165ce1aa6680e")   
    }

    search = GoogleSearch(params)         

    images_is_present = True
    while images_is_present:
        results = search.get_dict()      
        
        if "error" not in results:
            for image in results["images_results"]:
                if image["original"] not in image_results:
                    print(image["original"])
                    image_results.append(image["original"])
                       
            params["ijn"] += 1
        else:
            images_is_present = False
            print(results["error"])

print(json.dumps(image_results, indent=2))
print(len(image_results))

############################# Bathtubs and Whirlpools images ########################################

image_results = []
for query in ["Bathtubs and Whirlpools"]:
    params = {
        "engine": "google",               
        "q": query,                       
        "tbm": "isch",                     
        "num": "100",                     
        "ijn": 0,                         
        "api_key":("7981ea25ecca5cd1a09a815df3c8c1d9153924808ea2fe60ccd165ce1aa6680e")   
    }
    search = GoogleSearch(params)         

    images_is_present = True
    while images_is_present:
        results = search.get_dict()       
       
        if "error" not in results:
            for image in results["images_results"]:
                if image["original"] not in image_results:
                    print(image["original"])
                    image_results.append(image["original"])
                      
            params["ijn"] += 1
        else:
            images_is_present = False
            print(results["error"])

print(json.dumps(image_results, indent=2))
print(len(image_results))

############################# Showers images ########################################

image_results = []
for query in ["Showers"]:
    params = {
        "engine": "google",               
        "q": query,                       
        "tbm": "isch",                   
        "num": "100",                     
        "ijn": 0,                         # 
        "api_key":("7981ea25ecca5cd1a09a815df3c8c1d9153924808ea2fe60ccd165ce1aa6680e")   
    }

    search = GoogleSearch(params)         
    images_is_present = True
    while images_is_present:
        results = search.get_dict()       
    
        if "error" not in results:
            for image in results["images_results"]:
                if image["original"] not in image_results:
                    print(image["original"])
                    image_results.append(image["original"])      
            
            params["ijn"] += 1
        else:
            images_is_present = False
            print(results["error"])

print(json.dumps(image_results, indent=2))
print(len(image_results))
