## Hi there I'm Franklin👋

<!--
**Franklinj900/Franklinj900** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
# About me

**Description:**

**Tecnologías Utilizadas:**

* **NLTK;** 
* **Pandas;** 
* **Scikit-learn;** 
* **TensorFlow/Keras;** 

**Estructura del Proyecto:**

* **data:** 
* **notebooks:** 
* **models:** 
* **src:**

**Introducing me:**

```python
class DataScientist:
    """
    Represents a data scientist with Python skills.
    """
    def __init__(self, name, tech, hobbies):
        self.name = name
        self.tech = tech
        self.hobbies = hobbies

    def introduce_myself(self):
        print(f"Hello, I'm {self.name} and I'm a data scientist.")
        print(f"I work with technologies like: {', '.join(self.tech)}")
        print(f"My interests include: {', '.join(self.hobbies)}")

# Create an instance for yourself
me = DataScientist("Franklin José Ramos Gutierrez", ["FastAPI", "Pandas", "Scikit-learn"], ["Machine Learning", "Data Analysis", "Data Visualization"])

me.introduce_myself()
