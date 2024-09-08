# sensors.js

## Overview
`sensors.js` is a Node.js parser for `lm-sensors`, a command-line utility that provides information about the temperature, voltage, and fan speed of various hardware components. This library allows developers to easily integrate sensor data into their Node.js applications, enabling monitoring and management of system hardware.

## Features
- **Real-time Data Access**: Retrieve current sensor readings for temperature, voltage, and fan speeds.
- **Cross-Platform Support**: Works on any platform that supports Node.js and `lm-sensors`.
- **Easy Integration**: Simple API for integrating sensor data into your applications.

## Installation
To install `sensors.js`, you can use npm:

npm install sensors.js

## Usage
Here’s a simple example of how to use `sensors.js` in your Node.js application:

const sensors = require('sensors.js');

sensors.read((err, data) => {
    if (err) {
        console.error('Error reading sensors:', err);
        return;
    }
    console.log('Sensor Data:', data);
});

## API
### `sensors.read(callback)`
- **Description**: Reads the current sensor data.
- **Parameters**:
  - `callback`: A function that takes two arguments, `err` and `data`.
    - `err`: An error object if an error occurred, otherwise `null`.
    - `data`: An object containing the sensor readings.

## Contributing
Contributions are welcome! If you have suggestions for improvements or new features, please open an issue or submit a pull request.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments
- Thanks to the `lm-sensors` project for providing the underlying functionality.
- Special thanks to the contributors and community for their ongoing support.

## Contact
For any inquiries or feedback, please contact the maintainers through the repository's issue tracker.
