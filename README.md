# Webcam Image Classifier

A hands-on mini project that builds a convolutional neural network (CNN) and then puts it to work. You train a small image classifier on the CIFAR-100 dataset, then feed it a new picture, ideally one you capture with your webcam, and let the model predict what the picture shows. It is a short, practical introduction to the core ideas of deep learning for images.

## Learning Objectives

By the end of this repository, you should be able to:

- Build and train a simple CNN on the CIFAR-100 image dataset.
- Prepare image data (normalisation and resizing) for a neural network.
- Evaluate a classifier and read its training history.
- Apply a trained model to a new image and interpret the prediction.
- Save a trained model and reload it for later use.

## Learning Path

The project has two parts. Start with the assignment brief, then work through the notebook in order.

| File | Description |
|---|---|
| [**Assignment**](01_assignment.md) | The project brief: the two parts, what to build, and the deliverables. |
| [**Starter Notebook**](02_starter_notebook.ipynb) | Scaffolded notebook for Part A (train a CNN) and Part B (apply it to your own image). |

### Additional Folders and Files

| File / Folder | Description |
|---|---|
| [**Solutions**](solutions/) | Worked solution for the notebook. |
| [**pyproject.toml**](pyproject.toml) | Project configuration and dependencies. |
| [**uv.lock**](uv.lock) | Pinned dependency versions. |

## Setup

> [!NOTE]
> Throughout these steps, text in angle brackets like `<repo-name>` is a **placeholder**. Replace it, including the `< >` brackets, with your own value. For example, `cd <repo-name>` becomes `cd ds-image_classification_mini_project`.

### 1. Create the Repository from the Template

Click **Use this template** on GitHub.

When creating the repository:

- Set yourself as the **Owner**
- Choose a repository name
- Disable **Include all branches**
- Click **Create repository**

> [!IMPORTANT]
> If you are working in pairs or groups, only **one person** should complete this step.

---

### 2. Add Collaborators (Pairs/Groups Only)

If working with teammates:

1. Open the repository on GitHub
2. Go to **Settings → Collaborators**
3. Add your teammates as collaborators
4. Share the repository link with your team

Teammates should accept the invitation before continuing.

---

### 3. Clone the Repository

Copy the SSH URL from the **Code** button on GitHub, then run:

```bash
git clone <copied-ssh-url>
```

The copied SSH URL will look like `git@github.com:<your-username>/<repo-name>.git`.

---

### 4. Move into the Project Folder and Install Dependencies

This installs all dependencies and creates a virtual environment in (`.venv/`).

```bash
cd <repo-name>
uv sync
```

---

### 5. Open the Notebook

> [!NOTE]
> Make sure you open VS Code from the project root so it automatically detects the environment created by uv sync.

Launch VS Code in the project root folder:

```bash
code .
```

Then open `02_starter_notebook.ipynb`, select the Python environment created by `uv sync` as the kernel, and start with Part A.

> [!TIP]
> The notebook loads CIFAR-100 from the TensorFlow Datasets Google Cloud Storage mirror (`try_gcs=True`), so the download does not depend on the original dataset server being available.

## References & Further Reading

- [**TensorFlow CNN tutorial**](https://www.tensorflow.org/tutorials/images/cnn): Build and train a CNN image classifier with Keras.
- [**CIFAR-100 on TensorFlow Datasets**](https://www.tensorflow.org/datasets/catalog/cifar100): The dataset this project uses (100 classes of 32x32 colour images).
- [**CNN Explainer**](https://poloclub.github.io/cnn-explainer/): An interactive visualisation of how a CNN processes an image layer by layer.
- [**bonartm/imageclassifier**](https://github.com/bonartm/imageclassifier): A small webcam capture tool you can use to take the picture for Part B.
