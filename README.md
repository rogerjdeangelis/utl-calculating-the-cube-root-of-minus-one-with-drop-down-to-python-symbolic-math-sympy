# utl-calculating-the-cube-root-of-minus-one-with-drop-down-to-python-symbolic-math-sympy
    Calculate-the-three-cube-roots-of-minus-one-python-sympy;                                        
                                                                                                     
    Problem:                                                                                         
                                                                                                     
         Solve for x and y where                                                                     
                                                                                                     
         (x+I*y)**3 = -1                                                                             
                                                                                                     
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
                                                                                                     
    [(-1, 0), (1/2, -sqrt(3)/2), (1/2, sqrt(3)/2)]                                                   
                                                                                                     
    *     _               _                                                                          
      ___| |__   ___  ___| | __                                                                      
     / __| '_ \ / _ \/ __| |/ /                                                                      
    | (__| | | |  __/ (__|   <                                                                       
     \___|_| |_|\___|\___|_|\_\                                                                      
                                                                                                     
    ;                                                                                                
                                                                                                     
    The length and direction of the vector in the complex plain                                      
                                                                                                     
    For a more rigorous check see                                                                    
    https://www.quora.com/What-is-the-cube-root-of-negative-1                                        
                                                                                                     
    Lets check  root (1/2, -sqrt(3)/2)                                                               
                                                                                                     
      Vector length = (1/2)**2 + (-sqrt(3)/2)**2*i**2   (i**2=1)                                     
                                                                                                     
                    = .25 + .75 = 1                                                                  
                                                                                                     
                    = sign is negative because vector in fouth quadrant                              
                                                                                                     
                                                                                                     
                                                                                                     
     You can use Euler equality to algebraically check the result:                                   
                                                                                                     
         e**(i*x) = cos(x)+i* sin(x)                                                                 
                                                                                                     
    *                                                                                                
     _ __  _ __ ___   ___ ___  ___ ___                                                               
    | '_ \| '__/ _ \ / __/ _ \/ __/ __|                                                              
    | |_) | | | (_) | (_|  __/\__ \__ \                                                              
    | .__/|_|  \___/ \___\___||___/___/                                                              
    |_|                                                                                              
    ;                                                                                                
                                                                                                     
                                                                                                     
    %utl_submit_py64("                                                                               
    from sympy import *;                                                                             
    x, y, z = symbols('x y z', real=True);                                                           
    sol = solve((x+I*y)**3 + 1, (x, y));                                                             
    print(sol);                                                                                      
    ");                                                                                              
                                                                                                     
                                                                                                     
    [(-1, 0), (1/2, -sqrt(3)/2), (1/2, sqrt(3)/2)]                                                   
                                                                                                     
                                                                                                     
                                                                                                     
