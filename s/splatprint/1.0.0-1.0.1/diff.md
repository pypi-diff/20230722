# Comparing `tmp/splatprint-1.0.0.tar.gz` & `tmp/splatprint-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splatprint-1.0.0.tar", last modified: Thu Jul 20 11:59:56 2023, max compression
+gzip compressed data, was "splatprint-1.0.1.tar", last modified: Fri Jul 21 22:03:10 2023, max compression
```

## Comparing `splatprint-1.0.0.tar` & `splatprint-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 11:59:56.533477 splatprint-1.0.0/
--rw-rw-rw-   0        0        0     1086 2023-07-20 08:48:23.000000 splatprint-1.0.0/LICENSE.md
--rw-rw-rw-   0        0        0      244 2023-07-20 11:59:56.532480 splatprint-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    11997 2023-07-20 11:57:23.000000 splatprint-1.0.0/README.md
--rw-rw-rw-   0        0        0       82 2023-07-20 09:45:32.000000 splatprint-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-20 11:59:56.533477 splatprint-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      500 2023-07-20 11:55:36.000000 splatprint-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-20 11:59:56.525502 splatprint-1.0.0/splatprint/
--rw-rw-rw-   0        0        0        0 2023-07-17 09:06:40.000000 splatprint-1.0.0/splatprint/__init__.py
--rw-rw-rw-   0        0        0     3187 2023-07-18 10:01:14.000000 splatprint-1.0.0/splatprint/macropreview.py
--rw-rw-rw-   0        0        0     9675 2023-07-20 11:47:34.000000 splatprint-1.0.0/splatprint/printpost.py
--rw-rw-rw-   0        0        0     2408 2023-07-19 10:16:40.000000 splatprint-1.0.0/splatprint/repairpost.py
--rw-rw-rw-   0        0        0     8980 2023-07-20 11:50:30.000000 splatprint-1.0.0/splatprint/splatprint.py
--rw-rw-rw-   0        0        0      154 2023-07-20 10:16:04.000000 splatprint-1.0.0/splatprint/test.py
-drwxrwxrwx   0        0        0        0 2023-07-20 11:59:56.531482 splatprint-1.0.0/splatprint.egg-info/
--rw-rw-rw-   0        0        0      244 2023-07-20 11:59:56.000000 splatprint-1.0.0/splatprint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2023-07-20 11:59:56.000000 splatprint-1.0.0/splatprint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 11:59:56.000000 splatprint-1.0.0/splatprint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-07-20 11:59:56.000000 splatprint-1.0.0/splatprint.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2023-07-20 11:59:56.000000 splatprint-1.0.0/splatprint.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-20 11:59:56.000000 splatprint-1.0.0/splatprint.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 22:03:10.687013 splatprint-1.0.1/
+-rw-rw-rw-   0        0        0     1086 2023-07-20 08:48:23.000000 splatprint-1.0.1/LICENSE.md
+-rw-rw-rw-   0        0        0      244 2023-07-21 22:03:10.686016 splatprint-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    11865 2023-07-21 21:58:09.000000 splatprint-1.0.1/README.md
+-rw-rw-rw-   0        0        0       82 2023-07-20 09:45:32.000000 splatprint-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-21 22:03:10.687013 splatprint-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      500 2023-07-21 21:21:51.000000 splatprint-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 22:03:10.682063 splatprint-1.0.1/splatprint/
+-rw-rw-rw-   0        0        0        0 2023-07-17 09:06:40.000000 splatprint-1.0.1/splatprint/__init__.py
+-rw-rw-rw-   0        0        0     3187 2023-07-18 10:01:14.000000 splatprint-1.0.1/splatprint/macropreview.py
+-rw-rw-rw-   0        0        0    11526 2023-07-21 21:56:08.000000 splatprint-1.0.1/splatprint/printpost.py
+-rw-rw-rw-   0        0        0     2408 2023-07-19 10:16:40.000000 splatprint-1.0.1/splatprint/repairpost.py
+-rw-rw-rw-   0        0        0     9031 2023-07-21 21:57:16.000000 splatprint-1.0.1/splatprint/splatprint.py
+-rw-rw-rw-   0        0        0      785 2023-07-21 21:53:18.000000 splatprint-1.0.1/splatprint/test.py
+drwxrwxrwx   0        0        0        0 2023-07-21 22:03:10.685018 splatprint-1.0.1/splatprint.egg-info/
+-rw-rw-rw-   0        0        0      244 2023-07-21 22:03:10.000000 splatprint-1.0.1/splatprint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2023-07-21 22:03:10.000000 splatprint-1.0.1/splatprint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 22:03:10.000000 splatprint-1.0.1/splatprint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-07-21 22:03:10.000000 splatprint-1.0.1/splatprint.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2023-07-21 22:03:10.000000 splatprint-1.0.1/splatprint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-21 22:03:10.000000 splatprint-1.0.1/splatprint.egg-info/top_level.txt
```

### Comparing `splatprint-1.0.0/LICENSE.md` & `splatprint-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `splatprint-1.0.0/README.md` & `splatprint-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 5. Run splatprint:
 
         splatprint -i "image.png"
 
     Additional flags are listed under "Usage" below.
 
-    Splatprint creates macros for printing on blank canvases (`nrm_macro.txt`) and all-black canvases (`inv_macro.txt`). Depending on post contents, one may be significantly faster than the other; splatprint will suggest which macro to use by comparing the file sizes of both.
+    Splatprint creates macros for printing on blank canvases (`nrm_macro.txt`) and all-black canvases (`inv_macro.txt`). Depending on post contents, one may be significantly faster than the other; splatprint will suggest which macro to use by comparing the print times of both.
 
     Previews of macro prints are generated as `nrm_preview.png` and `inv_preview.png`. Blue pixels represent pixels the cursor passes over but doesn't print, while black/white (depending on macro type) indicates any printed pixels.
 
 6. Open the Splatoon post interface in horizontal mode. If using the inverse macro, manually paint the canvas black (touchscreen with largest brush size); otherwise, clear the canvas by pressing on the left joystick. The macro will automatically set the brush to the smallest size and move the cursor to the top left, so cursor size/position doesn't matter. 
 
 7. Undock your Switch, as any change in HDMI input will drop inputs for a short period. If using a longer macro, you may want to remove the USB-C cable from the dock and plug it directly into the Switch.
 
@@ -62,15 +62,15 @@
 
     The repair macro will also take a screenshot and press - to save after printing.
 
 ## Why Splatprint?
 Splatprint is designed for higher reliability when printing complex posts, minimizing the need for manual touchups.
 
 - In fast mode (default), splatprint scans the contents of each column to minimize the amount of inputs used when printing. To reduce the effects of dropped inputs, if the last pixel in a column is located at the top or bottom of the canvas, it also sends extra up/down inputs to ensure the cursor is at the proper location.
-- Splatprint can also print in cautious mode which prints in full columns to minimize the effects of dropped inputs. Printing in columns (rather than rows) allows the cursor to be aligned more frequently, reducing the area of effect of dropped inputs. 
+- Splatprint can also print in cautious mode, printing in full columns to minimize the effects of dropped inputs. Printing in columns rather than rows reduces the area of effect of dropped inputs. 
 - In case of errors, splatprint supports taking a screenshot of the Splatoon post interface to generate a repair macro that fixes any incorrect pixels. This feature can also be used to tweak the original image without printing the image from scratch.
     
 - Splatprint can also save the post contents of a screenshot to a 320x120 image, allowing you to rough out a post on the touchscreen and polish it in an image editor (useful if you don't have a drawing tablet).
 
 ## Demonstration
 
 [insert images here]
@@ -78,35 +78,35 @@
 ## Usage
 ### Arguments
 
 You can view the help message by running `splatprint` without any arguments.
 
 Standard usage of splatprint is as follows:
 
-    `splatprint -i "input.png"`
+    splatprint -i "input.png"
 
 - `-i "input.png"`: Input image, with `"input.png"` being a 320x120 image of the post you want to print. Splatprint will convert the image to black and white automatically (based on luminance), but will not apply dithering for any RGB/grayscale images. This can be in any format supported by `Pillow`, but a lossless format (like `.png`) is recommended.
 
 - `-d [#]` (optional): Delay, in seconds. Indicates the amount of time a button is pressed, as well as the amount of time the macro waits before inputting another button press. If not specified, will use the default value of 0.1.
 
     Lowering this value will increase the speed of macro execution at the risk of more dropped inputs. If you're printing longer macros and have a stable connection, it may be useful to start with a smaller delay to print the bulk of the post and do a second pass in repair mode with the default value (this hasn't been tested, though).
 
 - `-c` (optional): Cautious. If enabled, splatprint will pass the cursor through the entire column of any columns that contain printable pixels rather than moving to the next column after reaching the last printable pixel. This reduces the effects of any dropped inputs, as splatprint sends extra inputs at the end of a column to ensure the cursor is aligned with the top/bottom of the image, but usually significantly increases print time. However, enabling this does significantly reduce macro generation time.
 
 - `-v` (optional): Verbose. If enabled, splatprint will print messages when the program generates a macro file or macro preview file. Splatprint will still recommend a macro to use with this flag disabled.
 
-- `-p` (optional): Print instructions. If enabled, splatprint will print post print instructions after generating the macros, including post setup and the commands for running the macro file with NXBT.
+- `-p` (optional): Print instructions. If enabled, splatprint will print post printing instructions after generating the macros, including post setup and the commands for running the macro file with NXBT.
 
 Repair mode usage is as follows:
 
     splatprint -i "input.png" -r "screenshot.jpg"
 
-- `-i "input.png"`: Input image, with `"input.png"` being the 320x120 image that splatprint will correct the post to. Usually the original image used to generate macro in normal operation, but you can also use a revised version of the original to make tweaks to the post. Supported formats and color space are identical to standard operation.
+- `-i "input.png"`: Input image, with `"input.png"` being the 320x120 image that splatprint will correct the post to. Usually the original image used to generate the macro in normal operation. Supported formats and color space are identical to standard operation.
 
-- `-r "screenshot.jpg"`: Runs splatprint in repair mode. This generates a macro file that targets any pixels that were inputted incorrectly in-game. `screenshot.jpg` is the image of the in-game post that needs to be corrected. Must either be a 1280x720 screenshot of the post interface, taken with the Switch's capture button, or a 320x120 image of the post. The images saved to the Switch's album after publishing a post are not supported.
+- `-r "screenshot.jpg"`: Runs splatprint in repair mode. This generates a macro file that targets any pixels that were inputted incorrectly in-game. `screenshot.jpg` is the image of the in-game post that needs to be corrected. Must be either a 1280x720 screenshot of the post interface, taken with the Switch's capture button, or a 320x120 image of the post. The images saved to the Switch's album after publishing a post are not supported.
 
     Screenshots should be taken with the canvas set horizontally, the brush size set to smallest, and the cursor placed in the top left. However, manual screenshots usually aren't needed; macros generated by splatprint will automatically save an appropriate screenshot at the end of execution. See "How to print" above for some details on how to best transfer the screenshot to your computer while minimizing compression.
 
 - `-c`, `-v`, and `-p` (optional): Function identically to standard operation.
 
     If the initial macro suffered from several dropped inputs due to an unstable connection, cautious mode (`-c`) is recommended.
```

### Comparing `splatprint-1.0.0/splatprint/macropreview.py` & `splatprint-1.0.1/splatprint/macropreview.py`

 * *Files identical despite different names*

### Comparing `splatprint-1.0.0/splatprint/printpost.py` & `splatprint-1.0.1/splatprint/printpost.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 
 def postprint(array, inputfname, inverse, delay, repair, cautious):
     #open input file
     inputfile = open(inputfname, 'w')
     #universal vars
+    printtime = 0
     delaystr = str(delay) + 's'
     inputrpt = 3    #input repeat, number of extra inputs to send at the end of a line
     move_down = '\nDPAD_DOWN ' + delaystr + '\n' + delaystr
     move_up = '\nDPAD_UP ' + delaystr + '\n' + delaystr
     move_right = '\nDPAD_RIGHT ' + delaystr + '\n' + delaystr
     ink = '\nA ' + delaystr + '\n' + delaystr
     erase = '\nB ' + delaystr + '\n' + delaystr
@@ -16,74 +17,86 @@
     if inverse == False and repair == False:
         array = np.invert(array)
 
     #set up initial delay and A press on connect screen
     inputfile.write('3.0s')
     inputfile.write('\nA ' + delaystr)
     inputfile.write('\n5.0s')
+    printtime += delay + 8
 
     #move to top left, switch to smallest brush
     inputfile.write('\nL ' + delaystr + '\n' + delaystr)
     inputfile.write('\nL ' + delaystr + '\n' + delaystr)
     inputfile.write('\nL ' + delaystr + '\n' + delaystr)
     inputfile.write('\nL ' + delaystr + '\n' + delaystr)
     inputfile.write('\nL ' + delaystr + '\n' + delaystr)
     inputfile.write('\nL_STICK@-100+100 5s' + '\n' + delaystr)
+    printtime += (11 * delay) + 5
 
 
     #---------------------
     #Fast mode
     if cautious == False:
         #define funcs
-        def movetopixel(cursor_index, pixel_index):
+        def movetopixel(cursor_index, pixel_index, printtime_mtp):
             if pixel_index < cursor_index:			#pixel is below cursor
                 #move cursor
                 while cursor_index != pixel_index:
                     inputfile.write(move_down)                 #rotating image 90 degrees clockwise, end of column array is top of image
+                    printtime_mtp += delay * 2
                     cursor_index -= 1               #move cursor down
                 if cursor_index == 0:               #align if cursor moved to bottom of column
                     for i in range(inputrpt):
                         inputfile.write(move_down)
+                        printtime_mtp += delay * 2
             elif pixel_index > cursor_index:			#pixel is above cursor
                 while cursor_index != pixel_index:
                     inputfile.write(move_up)
+                    printtime_mtp += delay * 2
                     cursor_index += 1
                 if cursor_index == 119:             #align if cursor moved to top of column
                     for i in range(inputrpt):
                         inputfile.write(move_up)
-            return cursor_index
+                        printtime_mtp += delay * 2
+            return cursor_index, printtime_mtp
             
-        def printpixel(current_row, cursor_index, repair, inverse):
+        def printpixel(current_row, cursor_index, repair, inverse, printtime_pp):
             if repair:
                 pixel_val = current_row[cursor_index]
                 if pixel_val == 1:
                     inputfile.write(erase)
+                    printtime_pp += delay * 2
                 elif pixel_val == 2:
                     inputfile.write(ink)
+                    printtime_pp += delay * 2
             elif inverse:    #printpixel() should only be called for nonzero pixels
                 inputfile.write(erase)
+                printtime_pp += delay * 2
             else:
                 inputfile.write(ink)
-            return
+                printtime_pp += delay * 2
+            return printtime_pp
 
         #vars
         cursor_index = 119    #cursor y value (given bottom left is (0,0))
 
         #process array
         for crtrow in array:    #row of 90 degree rotated array, so each column
             printablepx = np.nonzero(crtrow)     #number of printable pixels in row
             printpxlen = np.size(printablepx)    #how many printable pixels are in the column
 
             if printpxlen == 0:                  #blank column
                 inputfile.write(move_right)      #move to next column
+                printtime += delay * 2
 
             if printpxlen == 1:                  #if 1 pixel
-                cursor_index = movetopixel(cursor_index, printablepx[0])
-                printpixel(crtrow, cursor_index, repair, inverse)
+                (cursor_index, printtime) = movetopixel(cursor_index, printablepx[0], printtime)
+                printtime = printpixel(crtrow, cursor_index, repair, inverse, printtime)
                 inputfile.write(move_right)
+                printtime += delay * 2
             
             #if more than 2+
             if printpxlen > 1:
                 #find whether the top or bottom pixel is closest to the cursor y value
                 max_index = np.max(np.nonzero(crtrow))
                 min_index = np.min(np.nonzero(crtrow))
                 if cursor_index == min_index:
@@ -108,34 +121,39 @@
                         furthest_index = min_index
                         printdir = -1
                     else:
                         closest_index = min_index
                         furthest_index = max_index
                         printdir = 1
                 #move cursor, print pixels in column
-                cursor_index = movetopixel(cursor_index, closest_index)
+                (cursor_index, printtime) = movetopixel(cursor_index, closest_index, printtime)
                 while cursor_index != furthest_index:
                     if np.any((np.isin(printablepx, cursor_index))):    #if cursor location has printable pixel
-                        printpixel(crtrow, cursor_index, repair, inverse)
+                        printtime = printpixel(crtrow, cursor_index, repair, inverse, printtime)
                     if printdir == -1:
                         inputfile.write(move_down)
+                        printtime += delay * 2
                         cursor_index -= 1
                     else:
                         inputfile.write(move_up)
+                        printtime += delay * 2
                         cursor_index += 1
                 #at end of line
                 if np.any((np.isin(printablepx, cursor_index))):
-                    printpixel(crtrow, cursor_index, repair, inverse)
+                    printtime = printpixel(crtrow, cursor_index, repair, inverse, printtime)
                 if cursor_index == 0 and printdir == -1:      #cursor is at bottom of column, printing downwards
                     for i in range(inputrpt):                 #so dropped inputs don't botch the whole thing, just to be safe
                         inputfile.write(move_down)
+                        printtime += delay * 2
                 elif cursor_index == 119 and printdir == 1:   #cursor is at top of column, printing up
                     for i in range(inputrpt):                 
                         inputfile.write(move_up)
+                        printtime += delay * 2
                 inputfile.write(move_right)                   #move to next column
+                printtime += delay * 2
 
 
     
     
     #---------------------
     #Cautious mode (kinda wack code but if it works)
     if cautious:
@@ -147,49 +165,66 @@
         for crtrow in array: #this iterates for every row in the 2d array
             #skip empty lines
             skip_line = False    #reset on new line
             if np.all(crtrow==0):     #if row is all non-printing (0 for repair, False for nrm/inv)
                 skip_line = True
             if skip_line:
                 inputfile.write(move_right)            #skip, move to next column
+                printtime += delay * 2
             #print the column
             if skip_line == False:    #skip extra processing if skipping line
                 if cur_mv_down:    #if moving top to bottom, need to flip the row
                     procrow = crtrow[::-1]    #flip current row, save as processed row
                 else:
                     procrow = crtrow    #if flipping isn't needed, make intact row the processed row
                 for x in procrow:    #iterate over the row
                     if repair:
                         if x == 1:
                             inputfile.write(erase)
+                            printtime += delay * 2
                         elif x == 2:    #2 == ink
                             inputfile.write(ink)
+                            printtime += delay * 2
                     elif inverse:    #if inverse, erase when True (white)
                         if x:
                             inputfile.write(erase)
+                            printtime += delay * 2
                     else:    #normal mode, ink when True (since flipped array)
                         if x:
                             inputfile.write(ink)
+                            printtime += delay * 2
                     inputfile.write(move_dir)
+                    printtime += delay * 2
             #runs at the end of the line
             if skip_line == False:
                 for i in range(inputrpt):    #send extra directional inputs to make sure cursor is at the edge
                     inputfile.write(move_dir)
+                    printtime += delay * 2
                 inputfile.write(move_right)    #move to next column
+                printtime += delay * 2
                 arypos += 1
                 if cur_mv_down:    #reverse input direction
                     cur_mv_down = False
                     move_dir = move_up
                 else:
                     cur_mv_down = True
                     move_dir = move_down
 
     #---------------------
 
     #move cursor to top, capture
     inputfile.write('\nL_STICK@-100+100 5s' + '\n' + delaystr)
-    inputfile.write('\nCAPTURE' + delaystr + '\n' + delaystr)
+    inputfile.write('\nCAPTURE ' + delaystr + '\n' + delaystr)
+    printtime += (delay * 3) + 5
 
     #save image and close file
     inputfile.write('\nMINUS ' + delaystr + '\n' + delaystr + '\n5.0s')
+    printtime += (delay * 2) + 5
     inputfile.close()
-    return
+
+    #process print time
+    printtime_div_ms = divmod(printtime, 60)    #divmod = divide w/ remainder
+    printtime_div_hm = divmod(printtime_div_ms[0], 60)
+    printtime_div = (printtime_div_hm[0], printtime_div_hm[1], printtime_div_ms[1])
+    printtime_str = ("{0:.0f}h {1:.0f}m {2:.2f}s".format(*printtime_div))    #{0}, {1}, etc. reference elements of unpacked tuple (*), :#f means # number precision fixed-point number
+
+    return printtime, printtime_str
```

### Comparing `splatprint-1.0.0/splatprint/repairpost.py` & `splatprint-1.0.1/splatprint/repairpost.py`

 * *Files identical despite different names*

### Comparing `splatprint-1.0.0/splatprint/splatprint.py` & `splatprint-1.0.1/splatprint/splatprint.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,16 +20,14 @@
     inv_preview_name = 'inv_preview.png'
     rpr_preview_name = 'rpr_preview.png'
     scr_name = 'proc_screenshot.png'    #1280x720 screenshot processed to 320x120
 
     #-----------------------------
     #Command line
 
-    possible_flags = ('-i', '-r', '-d', '-c', '-p', '-v', '-s')
-
     help_msg = '''Standard usage:
         img3splat -i "image.png"
     where "input.png" is the 320x120 image to print
 
     Repair mode:
         img3splat -i "image.png" -r "screenshot.jpg"
     "input.png" is the image to change the post to (320x120)
@@ -191,24 +189,24 @@
         if cautious:
             print('Printing in cautious mode!')
         else:
             print('Printing in fast mode!')
 
     #generate repair macro
     if repair:
-        postprint(proc_ar, rpr_macro_name, False, delay, True, cautious)
+        rpr_printtime, rpr_printtime_str = postprint(proc_ar, rpr_macro_name, False, delay, True, cautious)
         if verbose_en:
             print('Generated repair macro!')
 
     #generate normal/inverse macros
     else:
-        postprint(mainimg_ar, nrm_macro_name, False, delay, False, cautious)
+        nrm_printtime, nrm_printtime_str = postprint(mainimg_ar, nrm_macro_name, False, delay, False, cautious)
         if verbose_en:
             print('Generated macro!')
-        postprint(mainimg_ar, inv_macro_name, True, delay, False, cautious)
+        inv_printtime, inv_printtime_str = postprint(mainimg_ar, inv_macro_name, True, delay, False, cautious)
         if verbose_en:
             print('Generated inverse macro!')
 
     #------------------------------
     #run preview script
     if repair:
         preview(rpr_macro_name, rpr_preview_name, False, True, scrimg)
@@ -221,26 +219,26 @@
         preview(inv_macro_name, inv_preview_name, True, False, False)
         if verbose_en:
             print('Generated inverse macro preview!')
 
     #------------------------------
     #closing messages
 
-    #get smaller macro size
-    if repair == False:
-        nrm_size = os.path.getsize(nrm_macro_name)
-        inv_size = os.path.getsize(inv_macro_name)
-        if nrm_size < inv_size:
+    #show/compare print times
+    if repair:
+        print('Repair print time: ' + rpr_printtime_str)
+    else:
+        if nrm_printtime < inv_printtime:
             print('Normal macro likely has shorter print time.')
-            print('(' + str(nrm_size) + 'b vs. ' + str(inv_size) + 'b)')
-        elif nrm_size > inv_size:
+            print('(' + nrm_printtime_str + ' vs. ' + str(inv_printtime_str) + ')')
+        elif nrm_printtime > inv_printtime:
             print('Inverse macro likely has shorter print time.')
-            print('(' + str(inv_size) + 'b vs. ' + str(nrm_size) + 'b)')
+            print('(' + inv_printtime_str + ' vs. ' + nrm_printtime_str + ')')
         else:
-            print('Both macros have the exact same size (somehow).')
+            print('Both macros have the exact same size (' + nrm_printtime_str + ').')
 
     if print_instructions:
         print('''To print, open a blank plaza post (or all black if inverse),
     then press the "sync" button on your controller to disconnect it.
     Make sure your Switch is in handheld mode to prevent desyncs.''')
         if repair:
             print('''Then, run this command to start the print:
```

