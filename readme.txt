/* *****************************************************************************
 *  Name:    Misrach Ewunetie
 *  NetID:   ewunetie
 *  Precept: P10
 *
 *  Partner Name:    Eugenie Choi
 *  Partner NetID:   eyc2
 *  Partner Precept: P03
 *
 *  Hours to complete assignment (optional):
 *
 **************************************************************************** */

Programming Assignment 7: Seam Carving


/* *****************************************************************************
 *  Describe concisely your algorithm to find a horizontal (or vertical)
 *  seam.
 **************************************************************************** */
    We used the topological sort by going through the entirety of the distTo
    array we created. We found the minimum distTo values for each child. At the
    end, we found the index with the lowest distTo value at the last row. Using
    this, we then went through the edgeTo array and found the corresponding
    parents.


/* *****************************************************************************
 *  Describe what makes an image suitable to the seam-carving approach
 *  (in terms of preserving the content and structure of the original
 *  image, without introducing visual artifacts). Describe an image that
 *  would not work well.
 **************************************************************************** */
An image that would be suitable to the seam-carving approach might be one that
is all the same color or very similar colors. One that might not work well is one
with clearly defined edges, as this might distort the edges.


/* *****************************************************************************
 *  Perform computational experiments to estimate the running time to reduce
 *  a W-by-H image by one column and one row (i.e., one call each to
 *  findVerticalSeam(), removeVerticalSeam(), findHorizontalSeam(), and
 *  removeHorizontalSeam()). Use a "doubling" hypothesis, where you
 *  successively increase either W or H by a constant multiplicative
 *  factor (not necessarily 2).
 *
 *  To do so, fill in the two tables below. Each table must have 5-10
 *  data points, ranging in time from around 0.25 seconds for the smallest
 *  data point to around 30 seconds for the largest one.
 **************************************************************************** */

(keep W constant)
 W = 2000
 multiplicative factor (for H) =

 H           time (seconds)      ratio       log ratio
------------------------------------------------------
250                0.563
500                1.047           1.86
1000                2.074           1.98
2000                4.166           2.01
4000                9.669           2.21



(keep H constant)
 H = 2000
 multiplicative factor (for W) = 2

 W           time (seconds)      ratio       log ratio
------------------------------------------------------
250                0.635
500                1.091          1.71
1000               1.943          1.78
2000                3.818         1.96
4000                9.659         2.52



/* *****************************************************************************
 *  Using the empirical data from the above two tables, give a formula
 *  (using tilde notation) for the running time (in seconds) as a function
 *  of both W and H, such as
 *
 *       ~ 5.3*10^-8 * W^5.1 * H^1.5
 *
 *  Briefly explain how you determined the formula for the running time.
 *  Recall that with tilde notation, you include both the coefficient
 *  and exponents of the leading term (but not lower-order terms).
 *  Round each coefficient and exponent to two significant digits.
 **************************************************************************** */


Running time (in seconds) to find and remove one horizontal seam and one
vertical seam, as a function of both W and H:


    ~
       W^1 * H ^ 1.2




/* *****************************************************************************
 *  Known bugs / limitations.
 **************************************************************************** */
We ran out of time.

/* *****************************************************************************
 *  Describe whatever help (if any) that you received.
 *  Don't include readings, lectures, and precepts, but do
 *  include any help from people (including course staff, lab TAs,
 *  classmates, and friends) and attribute them by name.
 **************************************************************************** */
Lab TAs and Office Hour TA's on Saturday, Sunday, and Monday.

/* *****************************************************************************
 *  Describe any serious problems you encountered.
 **************************************************************************** */


/* *****************************************************************************
 *  If you worked with a partner, assert below that you followed
 *  the protocol as described on the assignment page. Give one
 *  sentence explaining what each of you contributed.
 **************************************************************************** */
Eugenie came up with ideas for code and wrote code.
Misrach also wrote code and thought of ways to implement code.

/* *****************************************************************************
 *  List any other comments here. Feel free to provide any feedback
 *  on how much you learned from doing the assignment, and whether
 *  you enjoyed doing it.
 **************************************************************************** */
:)
