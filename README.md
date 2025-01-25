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
