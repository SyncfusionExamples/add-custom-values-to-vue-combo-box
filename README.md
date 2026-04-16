# Add Custom Values to Vue Combo Box

## Repository Description
A Vue.js component enabling users to dynamically add custom values to combo box/select dropdown components with validation and real-time updates.

## Overview
This Vue component allows end-users to input and add custom values on-the-fly. Perfect for scenarios where the complete set of options cannot be predetermined.

## Features
- **Custom Value Input**: Add values not in the predefined list
- **Real-time Updates**: Dynamic dropdown option updates
- **Duplicate Validation**: Prevent duplicate entries
- **Easy Integration**: Simple API for Vue components
- **Customizable**: Configure when custom values are allowed
- **Accessible**: Maintains accessibility standards

## Prerequisites
- Node.js v12.0+
- Vue.js v2.6+ or v3.0+
- npm or yarn

## Installation
```bash
npm install add-custom-values-to-vue-combo-box
```

## Usage
```javascript
import VueComboBox from 'add-custom-values-to-vue-combo-box'

export default {
  components: { VueComboBox },
  data() {
    return {
      items: ['Option 1', 'Option 2'],
      selectedValue: null
    }
  }
}
```

## Configuration Options
- `allowCustomValues` - Enable custom value input (default: true)
- `validateDuplicates` - Prevent duplicates (default: true)
- `maxCustomValues` - Limit custom values count
- `placeholder` - Input placeholder text

## Example
```vue
<VueComboBox 
  v-model="selectedValue"
  :items="items"
  :allowCustomValues="true"
  placeholder="Select or add a value"
/>
```

## Contributing
Fork the repo, create a feature branch, and submit a pull request for contributions.

## License
MIT License - See LICENSE file for details.

## Support
Open an issue on the repository for questions or report bugs.
