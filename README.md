# COCO-JSON-to-YOLO-Bounding-Box

This Python script converts COCO (Common Objects in Context) dataset annotations in JSON format to YOLO (You Only Look Once) format. The YOLO format is commonly used for object detection tasks and is compatible with many deep learning frameworks.

## Features

- Loads COCO JSON annotations
- Creates a mapping from COCO category IDs to class names and indices
- Converts the bounding box coordinates from COCO format to YOLO format
- Saves the YOLO-formatted labels in a separate directory
- Copies the corresponding images to a separate directory
- Generates a `data.yaml` file with the necessary information for training a YOLO model


## Usage

1. Clone the repository:

   ```
   git clone https://github.com/SakibAhmedShuva/COCO-JSON-to-YOLO-Bounding-Box.git
   ```

2. Navigate to the project directory:

   ```
   cd COCO-JSON-to-YOLO-Bounding-Box
   ```

3. Open the `coco2yolo.ipynb` Jupyter Notebook.

4. Update the following variables with the appropriate paths:

   ```python
   coco_json_path = r'd:\OneDrive - Personal\instances_default.json'  # Adjust the path to your COCO JSON file
   output_dir = 'yolo'  # Output directory for YOLO-formatted data
   ```

5. Run the notebook to convert the COCO annotations to YOLO format.

6. The script will create the following directory structure in the `output_dir`:
   - `images`: Contains the copied image files
   - `labels`: Contains the YOLO-formatted label files
   - `data.yaml`: A YAML file with the necessary information for training a YOLO model

Sample data available in annotations and images folder.

## Requirements

- Python 3.x
- Jupyter Notebook
- `tqdm` library (`pip install tqdm`)

## Acknowledgements

This project was inspired by the need to convert COCO dataset annotations to a format compatible with YOLO object detection models.

## License

This project is licensed under the [MIT License](LICENSE).
