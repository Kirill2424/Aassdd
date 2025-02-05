# Aassdd
'''
import tkinter as tk
from tkinter import messagebox

def calculate_weight():
    try:
        height = float(height_entry.get())

        ideal_weight = height - 100

        result_label.config(text=f"Оптимальный вес: {ideal_weight:.2f} кг")

        if ideal_weight < float(weight_entry.get()):
            messagebox.showinfo("Рекомендация", "Вам нужно сбросить вес!")
        elif ideal_weight > float(weight_entry.get()):
            messagebox.showinfo("Рекомендация", "Вам нужно набрать вес!")
        else:
            messagebox.showinfo("Рекомендация", "Ваш вес в норме!")

    except ValueError:
        messagebox.showerror("Ошибка", "Пожалуйста, введите корректные числовые значения для роста и веса.")

# Создание главного окна
window = tk.Tk()
window.title("Определение Оптимального Веса")

# Метка и поле ввода для роста
height_label = tk.Label(window, text="Введите рост (см):")
height_label.pack()
height_entry = tk.Entry(window)
height_entry.pack()

# Метка и поле ввода для веса
weight_label = tk.Label(window, text="Введите вес (кг):")
weight_label.pack()
weight_entry = tk.Entry(window)
weight_entry.pack()

# Кнопка для расчета
calculate_button = tk.Button(window, text="Рассчитать", command=calculate_weight)
calculate_button.pack()

# Метка для вывода результата
result_label = tk.Label(window, text="")
result_label.pack()

window.mainloop()
'''
