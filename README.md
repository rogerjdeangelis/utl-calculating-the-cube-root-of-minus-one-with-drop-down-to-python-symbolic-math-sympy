# utl-calculating-the-cube-root-of-minus-one-with-drop-down-to-python-symbolic-math-sympy
Calculating the cube root of minus one with drop down to python symbolic math sympy package 

    Calculating the cube root of minus one with drop down to python symbolic math sympy package       
                                                                                                      
    Problem: Calculate the cube root of minus 1                                                       
                                                                                                      
    macros                                                                                            
    https://tinyurl.com/y9nfugth                                                                      
    https://github.com/rogerjdeangelis/utl-macros-used-in-many-of-rogerjdeangelis-repositories        
                                                                                                      
    *_                   _                                                                            
    (_)_ __  _ __  _   _| |_                                                                          
    | | '_ \| '_ \| | | | __|                                                                         
    | | | | | |_) | |_| | |_                                                                          
    |_|_| |_| .__/ \__,_|\__|                                                                         
            |_|                                                                                       
    ;                                                                                                 
    %let x=-1;                                                                                        
                                                                                                      
    *            _               _                                                                    
      ___  _   _| |_ _ __  _   _| |_                                                                  
     / _ \| | | | __| '_ \| | | | __|                                                                 
    | (_) | |_| | |_| |_) | |_| | |_                                                                  
     \___/ \__,_|\__| .__/ \__,_|\__|                                                                 
                    |_|                                                                               
    ;                                                                                                 
    SAS LOG                                                                                           
                                                                                                      
    Cube root of -1 is FROMPY=-1                                                                      
                                                                                                      
    *                                                                                                 
     _ __  _ __ ___   ___ ___  ___ ___                                                                
    | '_ \| '__/ _ \ / __/ _ \/ __/ __|                                                               
    | |_) | | | (_) | (_|  __/\__ \__ \                                                               
    | .__/|_|  \___/ \___\___||___/___/                                                               
    |_|                                                                                               
    ;                                                                                                 
                                                                                                      
                                                                                                      
    %utl_submit_py64("                                                                                
    from sympy import *;                                                                              
    import pyperclip;                                                                                 
    x = symbols('x');                                                                                 
    x=&x;                                                                                             
    r=x^(1/3);                                                                                        
    pyperclip.copy(r);                                                                                
    print r;                                                                                          
    ",return=fromPy);                                                                                 
                                                                                                      
    %put Cube root of -1 is &=frompy;                                                                 
                                                                                                      
