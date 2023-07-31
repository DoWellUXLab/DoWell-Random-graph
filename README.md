# DoWell-Random-graph

Welcome to the Random Graph API!. The Random Graph API provides two functionalities: Field Random Points and Excel Random Points. This API allows you to generate random points within a Cartesian plane and create random points based on an Excel-like grid. These features offer flexibility in generating random graphs for various applications.

## Features

The Random Graph API offers the following features:
1. Two functions: that are ```Field Random Points``` and ```Excel Random Points```.
2. Random Point Generation: The API generates random points within a Cartesian plane based on the provided parameters. It ensures that the generated points fall within the specified boundaries of the plane.
3. Starting Position Selection: You can choose the starting position within the Cartesian plane from where the random point generation begins. This allows you to control the location and orientation of the generated points.
4. Radius or Number of Points Selection: The API allows you to choose whether you want to specify the radius or the number of points to be generated. This flexibility accommodates different requirements and use cases.
5. Customizable Cartesian Plane: You can define the dimensions of the Cartesian plane by specifying the side length. The plane will be centered at the origin (0, 0) and extend to Â±side/2 on each axis.

## Getting Started

Getting Started with the Random Graph API's Key Features:

### ```Field Random Points```
1. This request is a POST method
    ```
    http://100022.pythonanywhere.com/v2/fieldrp/<YOUR-API-KEY>/
    ```
2. It sends a request body in JSON format with the following parameters:
    ```json
    {
        "side": 100,
        "selection": 5,
        "choice": 0,
        "value": 10
    }
    ```
3. The response body contains a JSON object with the following properties:
    ```json
    {
        "input_data": {
            "side": 100,
            "selection": 5,
            "choice": 0,
            "value": 10
        },
        "listOfPoints": [
            [
                0.0,
                -50.0
            ],
            [
                -25.52297676729542,
                -25.063737215226876
            ],
            [
                34.14062194962708,
                -39.62418785695287
            ],
            [
                21.67777066559354,
                -21.657208964092913
            ],
            [
                12.013646607068841,
                -16.400716675267816
            ],
            [
                -18.991085728674772,
                -19.791090592653163
            ],
            [
                34.491270056136585,
                -40.85714297115947
            ],
            [
                -23.49416380702403,
                -23.143644853705762
            ],
            [
                -12.503982474978494,
                -16.58009624489332
            ],
            [
                -34.12630387593561,
                -39.577191908968814
            ]
        ],
        "success": true
    }
    ```
### ```Excel Random Points```
1. This request is also a POST method
    ```json
    http://100022.pythonanywhere.com/v2/excelrp/<YOUR-API-KEY>/
    ```
2. It sends a request body in JSON format with the following parameters:
    ```json
    {
        "side":10,
        "selection":5
    }
    ```
3. The response body contains a JSON object with the following properties:
    ```json
    {
        "input_data": {
            "side": 10,
            "selection": 5
        },
        "listOfPoints": [
            [
                5.0,
                8.0
            ],
            [
                8.0,
                5.0
            ],
            [
                4.0,
                2.0
            ],
            [
                9.0,
                3.0
            ],
            [
                10.0,
                7.0
            ],
            [
                3.0,
                7.0
            ],
            [
                7.0,
                8.0
            ],
            [
                2.0,
                9.0
            ],
            [
                6.0,
                6.0
            ],
            [
                1.0,
                10.0
            ]
        ],
        "success": true
    }
    ```
## Documentation and Support

For detailed API documentation, including endpoint descriptions, request and response examples, and authentication details, please refer to the [API Documentation](https://documenter.getpostman.com/view/27523601/2s9XxsWGW2).

If you encounter any issues, have questions, or need assistance with the Random Graph API, please contact our support team.
