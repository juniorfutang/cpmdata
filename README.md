Simple but powerful Segmentation and Edge detection code learned from CHEME 599 Spring 2021 @ University of Washington

Images analyzed were of Hela cells, "The line is named after and derived from cervical cancer cells taken on February 8, 1951, from Henrietta Lacks, a 31-year-old African-American mother of five, who died of cancer on October 4, 1951. The cell line was found to be remarkably durable and prolific, which allows it to be used extensively in scientific study."

Hela cells are rather irregular in shape & divide quite fast. We expect that more "well behaved" cells will be easier to analyze not just in this piece of code but also in the YOLOv5 component

cv2.connectedComponentsWithStats function information
https://docs.opencv.org/3.4/d3/dc0/group__imgproc__shape.html#ga107a78bf7cd25dec05fb4dfc5c9e765f
Skimage canny function information
https://scikit-image.org/docs/dev/auto_examples/edges/plot_canny.html
