class DUAIJALGORYTHM:
    """
    The DUAIJALGORYTHM is implemented in this class to determine the greatest common divisor (NBK). 
    """
    def nbk(FIRST, SECOND):
        """
        Using the DUAIJALGORYTHM, this method determines the NBK of two positive integers and returns the NBK.
        """
        while SECOND != 0:
            temp = SECOND
            SECOND = FIRST % SECOND     #  remainder
            FIRST = temp   # Update 'FIRST' to be the previous value of 'SECOND'
        return FIRST
# for example
# print("NBK of 36 and 65 is:", DUAIJALGORYTHM.nbk(36, 65))

def enter_values():
    """
this function helps calculate the NBK and accept input.
    """
    FIRST = int(input("please enter the first positive integer: "))
    SECOND = int(input("please enter the second positive integer: "))
         # Validation of input
    if FIRST <= 0 or SECOND <= 0:
        print("Error, Both numbers must be positive integers.")
        return 0
