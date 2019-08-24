# utl-position-of-A-in-AGT-adenine-guanine-thymine-DNA-subsequences
Frequency of the position of A in AGT - adenine guanine thymine DNA subsequences 
    Frequency of the position of A in AGT - adenine guanine thymine DNA subsequences                            
                                                                                                                
    github                                                                                                      
    https://tinyurl.com/y36cuckz                                                                                
    https://github.com/rogerjdeangelis/utl-position-of-A-in-AGT-adenine-guanine-thymine-DNA-subsequences        
                                                                                                                
    *_                   _                                                                                      
    (_)_ __  _ __  _   _| |_                                                                                    
    | | '_ \| '_ \| | | | __|                                                                                   
    | | | | | |_) | |_| | |_                                                                                    
    |_|_| |_| .__/ \__,_|\__|                                                                                   
            |_|                                                                                                 
    ;                                                                                                           
                                                                                                                
    options validvarname=upcase;                                                                                
    libname sd1 "d:/sd1";                                                                                       
    data sd1.have;                                                                                              
      input (x1-x15) ($2.);                                                                                     
    cards4;                                                                                                     
    G T A T G T G T A G A T G A G                                                                               
    T A T G G G G T G G G G T G T                                                                               
    G G A G A T T G G T A G G A A                                                                               
    A G A G G A G G G G G T A G A                                                                               
    T G A G G A G A A T A G G T A                                                                               
    T G T T A G T T G T G T A G G                                                                               
    T T T T G T T T T A T A T T T                                                                               
    T A G T A T T G G T A G G G .                                                                               
    G A G G T A G G G T T . . A .                                                                               
    G A A G G G G G T . . . . G .                                                                               
    . G A G A . . T T . . . . G .                                                                               
    . G A . . . . G T . . . . A .                                                                               
    . G A . . . . T A . . . . T .                                                                               
    . T A . . . . . . . . . . G .                                                                               
    . A T . . . . . . . . . . . .                                                                               
    ;;;;                                                                                                        
    run;quit;                                                                                                   
                                                                                                                
                                                            | RULES                                             
                                                                        Frequency of                            
    Obs X1 X2 X3 X4 X5 X6 X7 X8 X9 X10 X11 X12 X13 X14 X15  | Position  'A's                                    
                                                            |                                                   
      1 G  T  A  T  G  T  G  T  A   G   A   T   G   A   G   |  1         4   X3,X9,X11, and X14                 
      2 T  A  T  G  G  G  G  T  G   G   G   G   T   G   T   |  2         1                                      
      3 G  G  A  G  A  T  T  G  G   T   A   G   G   A   A   |  3         5                                      
      4 A  G  A  G  G  A  G  G  G   G   G   T   A   G   A   |  4         5                                      
      5 T  G  A  G  G  A  G  A  A   T   A   G   G   T   A   |  5         6                                      
      6 T  G  T  T  A  G  T  T  G   T   G   T   A   G   G   |  6         2                                      
      7 T  T  T  T  G  T  T  T  T   A   T   A   T   T   T   |  7         2                                      
      8 T  A  G  T  A  T  T  G  G   T   A   G   G   G       |  8         3                                      
      9 G  A  G  G  T  A  G  G  G   T   T           A       |  9         3                                      
     10 G  A  A  G  G  G  G  G  T                   G       | 10         2                                      
     11    G  A  G  A        T  T                   G       | 11         2                                      
     12    G  A              G  T                   A       | 12         2                                      
     13    G  A              T  A                   T       | 13         2                                      
     14    T  A                                     G       | 14         1                                      
     15    A  T                                             | 15         1                                      
                                                                                                                
    *            _               _                                                                              
      ___  _   _| |_ _ __  _   _| |_                                                                            
     / _ \| | | | __| '_ \| | | | __|                                                                           
    | (_) | |_| | |_| |_) | |_| | |_                                                                            
     \___/ \__,_|\__| .__/ \__,_|\__|                                                                           
                    |_|                                                                                         
    ;                                                                                                           
                                                                                                                
    WORK.WANT total obs=15                                                                                      
                                                                                                                
      POS    CNTA                                                                                               
                                                                                                                
        1      4                                                                                                
        2      1                                                                                                
        3      5                                                                                                
        4      5                                                                                                
        5      6                                                                                                
        6      2                                                                                                
        7      2                                                                                                
        8      3                                                                                                
        9      3                                                                                                
       10      2                                                                                                
       11      2                                                                                                
       12      2                                                                                                
       13      2                                                                                                
       14      1                                                                                                
       15      1                                                                                                
                                                                                                                
    Frequency                                                                                                   
                                                                                                                
    6 +             XX                                                                                          
      |             XX                                                                                          
      |             XX                                                                                          
      |             XX                                                                                          
    5 +       XX XX XX                                                                                          
      |       XX XX XX                                                                                          
      |       XX XX XX                                                                                          
      |       XX XX XX                                                                                          
    4 + XX    XX XX XX                                                                                          
      | XX    XX XX XX                                                                                          
      | XX    XX XX XX                                                                                          
      | XX    XX XX XX                                                                                          
    3 + XX    XX XX XX       XX XX                                                                              
      | XX    XX XX XX       XX XX                                                                              
      | XX    XX XX XX       XX XX                                                                              
      | XX    XX XX XX       XX XX                                                                              
    2 + XX    XX XX XX XX XX XX XX XX XX XX XX                                                                  
      | XX    XX XX XX XX XX XX XX XX XX XX XX                                                                  
      | XX    XX XX XX XX XX XX XX XX XX XX XX                                                                  
      | XX    XX XX XX XX XX XX XX XX XX XX XX                                                                  
    1 + XX XX XX XX XX XX XX XX XX XX XX XX XX XX XX                                                            
      | XX XX XX XX XX XX XX XX XX XX XX XX XX XX XX                                                            
      | XX XX XX XX XX XX XX XX XX XX XX XX XX XX XX                                                            
      | XX XX XX XX XX XX XX XX XX XX XX XX XX XX XX                                                            
      -----------------------------------------------                                                           
         1  2  3  4  5  6  7  8  9 10 11 12 13 14 15                                                            
                                                                                                                
                            POS                                                                                 
                                                                                                                
    *                                                                                                           
     _ __  _ __ ___   ___ ___  ___ ___                                                                          
    | '_ \| '__/ _ \ / __/ _ \/ __/ __|                                                                         
    | |_) | | | (_) | (_|  __/\__ \__ \                                                                         
    | .__/|_|  \___/ \___\___||___/___/                                                                         
    |_|                                                                                                         
    ;                                                                                                           
                                                                                                                
    data want;                                                                                                  
     set sd1.have;                                                                                              
       pos=_n_;                                                                                                 
       cnta=countc(cats(of x:),"A");                                                                            
       drop x:;                                                                                                 
    run;quit;                                                                                                   
                                                                                                                
    options ls=64 ps=32;;                                                                                       
    proc chart data=want;                                                                                       
      vbar pos / discrete freq=cnta;                                                                            
    run;quit;                                                                                                   
                                                                                                                
