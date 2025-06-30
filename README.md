# Zettelkasten Plugin Documentation

## Overview

This Zettelkasten plugin transforms the Obsidian Svelte 5 template into a comprehensive knowledge management system inspired by Niklas Luhmann's Zettelkasten method. It features a modern neumorphism design and provides two main modes for organizing information.

## Features Implemented

### ✅ Core Components
- **ZettelkastenApp**: Main application component
- **Header**: Navigation between views
- **CardsView**: Grid-based card management
- **Card**: Individual knowledge cards with metadata
- **FlashNotesView**: Quick note-taking interface
- **FlashNote**: Individual flash notes with categories
- **FlashNoteEditor**: Modal editor for creating/editing notes
- **Toolbar**: Search and action controls

### ✅ State Management
- **viewStore**: Manages current view and UI state
- **cardsStore**: Handles card CRUD operations
- **searchStore**: Search functionality and filters
- **flashNotesStore**: Flash notes management

### ✅ Design System
- **Neumorphism**: Soft, elevated design with subtle shadows
- **CSS Variables**: Consistent color and spacing system
- **Responsive**: Mobile-friendly layouts
- **Dark/Light**: Theme support

### ✅ Functionality
- Create, edit, delete cards and flash notes
- Real-time search across content
- Color-coded categorization
- Tag-based organization
- Connection tracking between cards

## Usage Guide

### Getting Started

1. **Install Dependencies**:
   ```bash
   npm install
   ```

2. **Build the Plugin**:
   ```bash
   npm run build
   ```

3. **Test in Development**:
   ```bash
   npm run dev
   ```
   This builds and copies files to the test vault.

4. **Open Test Vault**:
   - Open `test-vault` folder in Obsidian
   - Enable the "Zettelkasten" plugin
   - Click the layers icon in the ribbon

### Card System

**Creating Cards**:
1. Switch to Cards view (grid icon)
2. Click the "+" button in toolbar
3. Add title, content, tags, and select color
4. Cards appear in a responsive grid layout

**Card Features**:
- Color indicators (blue, yellow, red, purple, green)
- Tag system for organization
- Connection tracking
- Creation/update timestamps
- Edit and delete actions

### Flash Notes

**Quick Capture**:
1. Switch to Flash Notes view (lightbulb icon)
2. Click the "+" button
3. Write content and select category
4. Save with Ctrl+Enter

**Categories**:
- 📝 **Notes**: General information
- ⚠️ **Important**: Critical items
- ✅ **Tasks**: Things to do
- 💡 **Inspiration**: Creative ideas

### Search & Organization

**Search Features**:
- Real-time text search
- Filter by tags and colors
- Sort by date or title
- Search suggestions

**Organization**:
- Use tags for grouping related content
- Color-code by topic or priority
- Connect related cards
- Archive completed items

## Technical Architecture

### Frontend Stack
- **Svelte 5**: Reactive UI with runes system
- **TypeScript**: Type safety and better DX
- **CSS Custom Properties**: Design system
- **Vite**: Fast build and development

### File Structure
```
src/
├── components/          # UI components
├── stores/             # State management
├── styles/             # CSS design system
├── views/              # Obsidian integration
├── types.ts            # Type definitions
└── main.ts             # Plugin entry
```

### Key Design Decisions

1. **Neumorphism**: Creates depth without harsh shadows
2. **Component Architecture**: Modular, reusable components
3. **Store Pattern**: Centralized state with reactive updates
4. **Type Safety**: Comprehensive TypeScript coverage
5. **Responsive Design**: Works on all screen sizes

## Development Notes

### Build Process
- TypeScript compilation with Svelte preprocessing
- CSS bundling with custom properties
- Asset optimization for Obsidian environment
- Source maps for debugging

### Testing Strategy
- Component isolation testing
- Store functionality verification
- Integration testing with test vault
- Cross-platform compatibility

### Performance Considerations
- Lazy loading of components
- Efficient search algorithms
- Minimal re-renders with Svelte stores
- Optimized CSS with custom properties

## Future Enhancements

### Planned Features
- [ ] Graph view for card connections
- [ ] Export/import functionality
- [ ] Advanced filtering options
- [ ] Keyboard shortcuts
- [ ] Plugin settings panel
- [ ] Integration with Obsidian notes
- [ ] Backup and sync capabilities

### Technical Improvements
- [ ] Virtual scrolling for large datasets
- [ ] Offline storage optimization
- [ ] Performance monitoring
- [ ] Accessibility enhancements
- [ ] Mobile app support

## Troubleshooting

### Common Issues

1. **Plugin Not Loading**:
   - Check manifest.json is valid
   - Ensure all files are in correct directory
   - Verify Obsidian version compatibility

2. **Build Errors**:
   - Run `npm run check` for type errors
   - Check import paths are correct
   - Verify all dependencies are installed

3. **Styling Issues**:
   - Check CSS custom properties are defined
   - Verify component styles are scoped
   - Test in different themes

### Debug Mode
Enable debug logging by setting `console.log` statements in stores and components. The browser dev tools can be accessed in Obsidian for debugging.

## Contributing

### Development Workflow
1. Fork the repository
2. Create feature branch
3. Make changes with tests
4. Run quality checks
5. Submit pull request

### Code Standards
- Use TypeScript for all new code
- Follow Svelte 5 best practices
- Maintain consistent styling
- Add JSDoc comments for public APIs
- Test on multiple screen sizes

This plugin demonstrates a complete implementation of a modern Obsidian plugin using Svelte 5, showcasing advanced UI patterns, state management, and integration with Obsidian's ecosystem.
# obsidian-Zettelkasten
