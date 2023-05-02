Download Link: https://assignmentchef.com/product/solved-cpe301-homework-2-declaration-statements
<br>
<ol>

 <li>Write declaration statements (for Atmega2560 volatile data) for the following.

  <ol>

   <li>The variable pointed to by y addr is an integer.</li>

   <li>The variable pointed to by ch_addr is an unsigned character.</li>

   <li>The variable pointed to by z is an integer.</li>

   <li>date_pt is a pointer to an integer.</li>

   <li>pt_chr is a pointer to an unsigned character.</li>

  </ol></li>

 <li>For the following declarations,</li>

</ol>

int *x_pt, *y_addr; long *dt_addr, *pt_addr;

double *pt_z; int a; long b; double c;

Determine which of the following statements is valid.

<table width="0">

 <tbody>

  <tr>

   <td width="192">a. y_addr = &amp;a;</td>

   <td width="192">b. y_addr = &amp;b;</td>

   <td width="176">c. y_addr = &amp;c;</td>

  </tr>

  <tr>

   <td width="192">d. y_addr = a;</td>

   <td width="192">e. y_addr = b;</td>

   <td width="176">f. y_addr = c;</td>

  </tr>

  <tr>

   <td width="192">g. dt_addr = &amp;a;</td>

   <td width="192">h. dt_addr = &amp;b;</td>

   <td width="176">i. da_addr = &amp;c;</td>

  </tr>

  <tr>

   <td width="192">j. dt_addr = a;</td>

   <td width="192">k. dt_addr = b;</td>

   <td width="176">l. dt_addr = c;</td>

  </tr>

  <tr>

   <td width="192">m. pt_z = &amp;a;</td>

   <td width="192">n. pt_addr = &amp;b;</td>

   <td width="176">o. pt_addr = &amp;c;</td>

  </tr>

  <tr>

   <td width="192">p. pt_addr = a;</td>

   <td width="192">q. pt_addr = b;</td>

   <td width="176">r. pt_addr = c;</td>

  </tr>

  <tr>

   <td width="192">s. y_addr = x_pt;</td>

   <td width="192">t. y_addr = dt_addr;</td>

   <td width="176">u. y_addr = pt_addr;</td>

  </tr>

 </tbody>

</table>

<ol start="3">

 <li>If a variable is declared as a pointer, what must be stored in the variable?</li>

 <li>if var2 is a variable, what does &amp;var2 mean?</li>

 <li>Using the sizeof ( ) operator, determine the number of bytes used by your PC to store the address of an integer, character, and double precision number. (Hint: sizeof (*int) can be used to determine the number of memory bytes used for a pointer to an integer.) Would you expect the size of each address to be the same? Why or why not?</li>

 <li>Determine the results of the following operations:

  <ol>

   <li>11001010 11001010     c. 11001010  <u>&amp; 10100101</u>     <u>| 10100101</u>      <u>^ 10100101</u></li>

  </ol></li>

 <li>Write the hexadecimal representations of all binary numbers in Question 6.</li>

 <li>Determine the binary and hexadecimal results of the following operations, assuming unsigned numbers:

  <ol>

   <li>the hexadecimal number 0x0157, shifted left by one bit position</li>

   <li>the hexadecimal number 0x0701, shifted left by two bit positions</li>

   <li>the hexadecimal number 0x0673 shifted right by two bit positions</li>

   <li>the hexadecimal number 0x0057 shifted right by three bit positions</li>

  </ol></li>

 <li>Assume that the arbitrary bit pattern xxxxxxxx, where each x can represent either 1 or 0, is stored in the integer variable named flag. Determine the hexadecimal value of a mask that can be ANDed with the bit pattern to reproduce the third and fourth bits of flag and set all other bits to zero. The rightmost bit in flag is considered bit 0.

  <ol>

   <li>Determine the hexadecimal value of a mask that can be inclusively ORed with the bit pattern in f1ag to reproduce the fifth and seventh bits of flag and set all other bits to one. Again, consider the rightmost bit of flag to be bit 0.</li>

   <li>Determine the hexadecimal value of a mask that can be used to complement the values of the first and third bits of f1ag and leave all other bits unchanged. Determine the bit operation that should be used with the mask value to produce the desired result.</li>

  </ol></li>

 <li>The BIOS (Basic Input Output Services) controls low level I/O on a computer. When a (PC) computer first starts up the system BIOS creates a data area starting at memory address 0x400 for its own use.</li>

</ol>

Address 0x0417 is the Keyboard shift flags register, the bits of this byte have the following meanings:

Bit       Value               Meaning

<table width="0">

 <tbody>

  <tr>

   <td width="48">7</td>

   <td width="48">0/1</td>

   <td width="154">Insert               off/on</td>

  </tr>

  <tr>

   <td width="48">6</td>

   <td width="48">0/1</td>

   <td width="154">CapsLock        off/on</td>

  </tr>

  <tr>

   <td width="48">5</td>

   <td width="48">0/1</td>

   <td width="154">NumLock        off/on</td>

  </tr>

  <tr>

   <td width="48">4</td>

   <td width="48">0/1</td>

   <td width="154">ScrollLock      off/on</td>

  </tr>

  <tr>

   <td width="48">3</td>

   <td width="48">0/1</td>

   <td width="154">Alt key            up/down</td>

  </tr>

  <tr>

   <td width="48">2</td>

   <td width="48">0/1</td>

   <td width="154">Control key     up/down</td>

  </tr>

  <tr>

   <td width="48">1</td>

   <td width="48">0/1</td>

   <td width="154">Left shift key up/down</td>

  </tr>

  <tr>

   <td width="48">0</td>

   <td width="48">0/1</td>

   <td width="154">Right shift key up/down</td>

  </tr>

 </tbody>

</table>

This byte can be written as well as read. Thus we may change the status of the CapsLock, NumLock and ScrollLock LEDs on the keyboard by setting or clearing the relevant bit.

Write a C function using pointers and bit operators to turn Caps lock on without changing the other bits. NOTE: Do NOT try to execute this on your PC unless you boot it to DOS in real mode.

(Portions of these Questions are modified from: “C++ for Engineers and Scientists” by Gary Bronson, and http://www.scs.ryerson.ca/~mth110/Handouts/bitwise.pdf)