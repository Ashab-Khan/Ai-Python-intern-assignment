# 🧠 AI Python Intern Assignment
This project is a Colab-based tool that extracts questions and their associated images from a multi-page educational PDF. It automatically identifies:

Question text (e.g., "1. Find the next figure...")

Related image(s) for the question

Option images ([A], [B], [C], [D]) if present

The output is saved in a JSON format suitable for quizzes, e-learning, or data labeling use.

✅ Features
    📄 Extracts questions from PDF pages using regex

    🖼 Extracts and saves images with bounding box position

    📌 Associates images with the nearest question using Y-axis matching

✅ Applies smart rules:

    If 4 images → all are options

    If >4 → last 4 are options, rest are question diagrams

    If <4 → all images belong to the question

    🔄 Converts question_images to a single string "images" (your desired format)

    🗃 Saves output to questions_with_images.json

    📦 Zips all extracted images for easy download


📁 Folder Structure (after running the script)

    /images/
    page1_img1.png
    page1_img2.png
    ...
    questions_with_images.json
    images.zip