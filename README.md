🦋 Butterfly Wing Motion Tracker (Dense Optical Flow)
This project tracks and visualizes the motion of butterfly wings using dense optical flow.
It precisely isolates fast wing movements by applying a custom mask around the butterfly and filters out background noise like leaves and flowers.
All outputs are automatically saved inside your Google Drive.

📂 Project Structure
Dense Optical Flow (Farneback) method for pixel-wise motion tracking.

ROI Masking: Focus only on the butterfly region.

Motion Thresholding: Visualize only fast movements (wing beats).

Video Output: Saves the processed motion video as .mp4.

Google Drive Saving: Results are directly saved into Drive folders.

🚀 How It Works
Mounts your Google Drive.

Loads input video.

Crops video between 14s and 20s.

Computes dense optical flow on each frame.

Applies a mask to restrict tracking to the butterfly area.

Filters out slow/static motions.

Generates and saves a motion visualization video.

🛠️ Requirements
Python 3.x

OpenCV

Google Colab (or local environment with Drive API access)

Install required libraries:

bash
Copy
Edit
pip install opencv-python
If using Google Colab, no extra installations are needed except mounting Google Drive.

📋 How To Run
Clone this repository or copy the code into your Colab notebook.

Make sure your butterfly video (Butterflywing.mp4) is stored in your Drive:

swift
Copy
Edit
/MyDrive/Butterfly Motion Track/Butterflywing.mp4
Run the script:

python
Copy
Edit
analyze_butterfly('/content/drive/MyDrive/Butterfly Motion Track/Butterflywing.mp4')
Outputs will be saved automatically under:

swift
Copy
Edit
/MyDrive/ButterflyDenseTrackingResults/results_XXXX/
Files generated:

butterfly_wing_motion_masked.mp4 (main motion visualization video)

📊 Example Result
Only the butterfly wings in motion are visualized.

Background and non-moving parts are masked out.

Video output shows dynamic wing beating captured frame-by-frame.

✨ Future Improvements
Automatic butterfly detection using deep learning.

Adaptive thresholding based on wing speed.

3D optical flow visualization for advanced studies.

📜 License
This project is released under the MIT License.

