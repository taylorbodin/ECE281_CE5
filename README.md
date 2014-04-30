ECE281_CE5
==========

MIPS for days

##Task 1

```
# MIPS task one which initializes two registers, adds them, and stores the result to memory
# C3C Bodin

main:
      li        $s0, 44 # Load Register $s0 with 44
      li        $s1, -31 # Load Register $s1 with -31
      add       $s2,$s1,$s0 # Put the result of $s1 + $s0 in $s2
      sw        $s2, 10($s0) # Store $s2 to 44 + and offset of 10 i.e. x54
      
```
