ECE281_CE5
==========

MIPS for days

##Task 1

```
# MIPS task one which initializes two registers, adds them, and stores the result to memory
# C3C Bodin

main:
      addi      $s0,$0,44 # Load Register $s0 with 44
      addi      $s1,$0,-31 # Load Register $s1 with -31
      add       $s2,$s1,$s0 # Put the result of $s1 + $s0 in $s2
      sw        $s2, 54($0) # Store $s2 to 0 + and offset of 54 i.e. x54
      
```

##Task 2

```
# MIPS task one which initializes two registers, adds them, and stores the result to memory
# C3C Bodin

main:
      addi      $s0,$0,44 # 0x2010002C
      addi      $s1,$0,-31 # 0x2011FFE1
      add       $s2,$s1,$s0 # 0x02309020
      sw        $s2, 54($0) # 0xAC120036
      
```

For some reason I just COULD NOT get the given wave form file. I've included the default wave form with
the radix changed for readability and annotated to show a working program. 

![alt text](task2.JPG "Stupid wave files")

As annotated on the waveform, the ALU out first held 44, then -34, and finally the result of 44+(-34) which is
13. Then the ALU out bus held the memory location 54 and writedata held 13 which is exactly what we wanted. 
