

# 🍳 DeepChef

**DeepChef** is an intelligent recipe recognition web app that identifies dishes from photos and suggests their recipes.
Upload an image of a dish, and DeepChef will recognize it using deep learning and return the top 5 most similar recipes!

---

## 🚀 Features

* **Image Upload Interface:** Click and upload any food image.
* **Dish Recognition:** Uses a pre-trained **DenseNet (Keras)** model to extract image features.
* **Recipe Retrieval:** Finds top 5 matching dishes using **cosine similarity (arccosine distance)** between image feature vectors.
* **Dataset:**

  * Scraped **380+ recipes** from [food.com](https://www.food.com).
  * Collected **10 images per dish** via **Google Images** using Selenium.
* **Web App:** Built using **Django**, **HTML**, **CSS**, and **JavaScript**.

---

## 🧠 Tech Stack

* **Backend:** Django
* **Frontend:** HTML, CSS, JavaScript
* **Deep Learning:** Keras with DenseNet
* **Web Scraping:** Selenium, BeautifulSoup

---

## ⚙️ How do we use it?

1. User uploads an image of a dish.
2. The image is passed through DenseNet to generate a feature vector.
3. These features are compared (via arccosine similarity) with precomputed features of the dataset.
4. The top 5 most similar dishes are displayed along with their recipes.

