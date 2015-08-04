
This is the docs for my phone number api. 

    >>> from phones import PhoneNumber

To create a number, you just provide it as a string or integer 

    >>> PhoneNumber(1112223333, 'home')
    [home] (111) 222-3333
    >>> PhoneNumber("1112223333", 'home')
    [home] (111) 222-3333
    
You can also add the optional '1' at the beginning:
    
    >>> PhoneNumber("11112223333", 'home')
    [home] (111) 222-3333
    
Parenthases, dashes or spaces are ignored:    

    >>> number = PhoneNumber("111-222-3333", 'home')
    >>> number
    [home] (111) 222-3333
    
If for any reason you need the raw number, and not the string representation, it's available like so:

    >>> number.raw_number
    '1112223333'