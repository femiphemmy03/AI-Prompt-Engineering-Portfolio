 
# Day 2: AI Prompt Engineering Portfolio

## Prompt 1: Python Code Snippet

**Prompt**: "Act as a Python tutor and generate a beginner-friendly code snippet to sort a list of numbers, with a 50-word explanation."

**Output**:  Create a list of numbers

numbers = [5, 2, 9, 1, 7]

 Sort the list in ascending order

numbers.sort()

Print the sorted list

print("Sorted numbers:", numbers)

Explanation:
This code creates a list of numbers and uses the built-in sort() method to arrange them in ascending order (from smallest to largest). It's efficient, easy to read, and perfect for beginners. You can also use numbers.sort(reverse=True) to sort in descending order. Simple and powerful!
Want to try it with your own list or explore how sorting works behind the scenes? 🧠💡

**Notes**: Prioritized beginner understanding by using clear variable names and the built-in .sort() method. Provided a concise 50-word explanation to reinforce concept learning. Ensured code was clean, functional, and executable for first-time learners.

## Prompt 2: Machine Learning Q&A

**Prompt**: "Answer the question 'What is machine learning?' in 100 words, tailored for a high school student."

**Output**: Machine learning is a way for computers to "learn" from data instead of being told exactly what to do. Imagine teaching a computer to recognize photos of cats—not by writing rules like "if it has whiskers," but by showing it many cat pictures. Over time, the computer finds patterns and gets better at spotting cats on its own. This is how apps recommend songs, translate languages, or predict weather. Machine learning helps machines make decisions based on experience—just like humans learn from practice. It’s a big part of artificial intelligence and is used in phones, games, websites, and even cars.

**Notes**: Explained machine learning using simple, relatable terms suitable for a high school student. Avoided technical jargon while connecting to everyday examples like photos, recommendations, and AI. Kept the tone engaging and informative within the 100-word limit..

## Prompt 3: FAQ for Tech Startup

**Prompt**: "Generate a 5-point FAQ for a tech startup’s new app, focusing on user benefits."

**Output**: 📱 App FAQ – Focused on User Benefits
1. What does the app help me do?

Our app simplifies your daily tasks by automating reminders, organizing your to-dos, and syncing across all your devices—helping you stay focused and productive.

2. Is the app easy to use for beginners?

Absolutely! The app features a clean interface, smart suggestions, and helpful tutorials to guide new users through setup and usage.

3. Will I save time using this app?

Yes. Users report saving up to 2 hours daily thanks to quick task creation, smart scheduling, and instant notifications.

4. Does the app work offline?

Yes, the core features work without internet access. Your data syncs automatically once you're back online.

5. How secure is my personal information?

We use end-to-end encryption and never share your data with third parties—your privacy and security are our top priorities.

**Notes**: Focused on concise, benefit-driven content for a professional audience.

## Prompt 4: Creative Writing

**Prompt**: "Generate a 3-paragraph short story that begins with someone discovering a mysterious map in their grandmother’s attic. Include elements of mystery and emotional depth."

**Output**: While cleaning out his late grandmother’s attic, Daniel found an old chest tucked beneath moth-eaten quilts and yellowed books. Inside was a rolled-up parchment sealed with faded wax and marked with strange symbols. When he unrolled it, he realized it was a map—but not of anywhere he recognized. At the bottom, in his grandmother’s handwriting, were the words: “To the place where we left the truth.” A cold shiver ran down his spine. His grandmother had always been eccentric, but this felt like something more—something hidden.

As Daniel studied the map, he noticed a location circled in red ink: a remote clearing just outside the town where his grandmother had grown up. He decided to follow it, driven by curiosity and a strange pull he couldn’t explain. The journey led him deep into the woods, where the trees whispered in the wind and the path felt older than time itself. There, in the clearing, he found a weathered stone bench and a small wooden box buried beneath it. Inside was a locket containing a photo of a man he’d never seen—standing beside his grandmother.

Back home, he found the same man in an old photo album labeled “What never was.” It was her first love, lost during the war, long presumed dead. With the map, she had kept the memory of their secret place alive, hidden from a world that had moved on. Daniel sat quietly in the attic, locket in hand, tears rising. He had unearthed more than a map—he’d uncovered a piece of her heart she’d never shared, and now it lived in him, too.

**Notes**: Crafted a short story that balances mystery (hidden map, unknown location, secret past) with emotional depth (loss, legacy, memory). The structure follows a clear beginning (discovery), middle (journey), and end (revelation), aimed at sparking both curiosity and sentiment.

## Prompt 5: Data Analysis Support

**Prompt**: "Act like a data analyst mentor. Given a dataset of sales by region (user will upload CSV), suggest three ways to visualize the data in Python with libraries like Matplotlib or Seaborn. Include sample code snippets."

**Output**: Absolutely, Oluwafemi! As your data analyst mentor, I’ll guide you on how to visualize a sales-by-region dataset using Python’s popular libraries—Matplotlib and Seaborn. Once you upload the CSV, I can give more tailored visuals, but here's a general approach you can apply immediately.
1. Bar Chart – Total Sales by Region

Why: Bar charts are perfect for comparing sales volumes across regions.

import pandas as pd

import matplotlib.pyplot as plt

Load data

df = pd.read_csv('sales_by_region.csv')

 Group by region and sum sales

region_sales = df.groupby('Region')['Sales'].sum().sort_values()

 Plot
 
region_sales.plot(kind='barh', color='skyblue')

plt.title('Total Sales by Region')

plt.xlabel('Sales Amount')

plt.ylabel('Region')

plt.tight_layout()

plt.show()

 Calculate share

region_sales = df.groupby('Region')['Sales'].sum()

Plot

region_sales.plot(kind='pie', autopct='%1.1f%%', startangle=140, figsize=(6,6))

plt.title('Sales Distribution by Region')

plt.ylabel('')

plt.show()

2. Pie Chart – Proportion of Sales per Region

Why: Pie charts help show each region’s percentage share of total sales.

Calculate share

region_sales = df.groupby('Region')['Sales'].sum()

 Plot

region_sales.plot(kind='pie', autopct='%1.1f%%', startangle=140, figsize=(6,6))

plt.title('Sales Distribution by Region')

plt.ylabel('')

plt.show()

3. Boxplot – Sales Distribution by Region

Why: Boxplots show spread, outliers, and median sales, great for identifying regional variability.

import seaborn as sns

plt.figure(figsize=(8, 5))

sns.boxplot(data=df, x='Region', y='Sales', palette='pastel')

plt.title('Sales Distribution by Region')

plt.xticks(rotation=45)

plt.tight_layout()

plt.show()

**Notes**: Suggested 3 visualization types aligned with key analysis goals—comparison (bar), proportion (pie), and distribution (box). Included beginner-friendly, ready-to-run code using pandas, Matplotlib, and Seaborn. Designed to support hands-on learning and immediate insight generation from a typical sales dataset.