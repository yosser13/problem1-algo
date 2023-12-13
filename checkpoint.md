ALGORITHM list
VAR
    a=[3,1,7,9]:INTEGER
    b=[2,4,1,9,3]:INTEGER
    som=0:INTEGER
BEGIN
    for i from 0 to long(a);
        test=false
    for j from 0 to long(b);
    IF (a[i]==a[j]) THEN
        test=true
    END_IF
    END_FOR
    IF (test==false) THEN
    som=som+a[i]  
    END_IF
    END_FOR

    for J from 0 to long(b);
        test=false
    for i from 0 to long(a);
    IF (a[i]==b[j]) THEN
        test=true
    END_IF
    END_FOR
    IF (test==false) THEN
    som=som+b[j]  
    END_IF
    END_FOR

    WRITE (som)
END