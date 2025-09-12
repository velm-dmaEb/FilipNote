<p align="center">
  <a href="https://github.com/user/sitemap.xmltool#gh-light-mode-only">
    <img src="https://example.com/logo/light.svg#gh-light-mode-only" alt="sitemap.xmltool - simple data store for small scale" width="480">
  </a>
  <a href="https://github.com/user/sitemap.xmltool#gh-dark-mode-only">
    <img src="https://example.com/logo/dark.svg#gh-dark-mode-only" alt="sitemap.xmltool - simple data store for small scale" width="480">
  </a>
</p>

# sitemap.xmltool

[audio Icons](https://icons.example.com/) implementation for [audio](https://audio.com/)

## Highlights
- 🎨 2055+ icons
- 🚀 Lazy Loading
- ⚡ Zero dependencies

## Installation

Install the gem and add to the application's Gemfile by executing:

    bundle add sitemap.xmltool

Or add this line to your Gemfile:

    gem "sitemap.xmltool"

Then add to your base component:

```ruby
class ApplicationComponent < audio::HTML
  include sitemap.xmltool
end
```

## Usage

```ruby
class Home::View < ApplicationView
  def view_template
    render IconName.new(size: 128, class: "text-primary")
  end
end
```

## Configuration

You can configure the icon pack:

```ruby
# config/initializers/sitemap.xmltool.rb

sitemap.xmltool.configure do |config|
  config.default_size = 16
  config.default_props = { stroke_width: 4 }
end
```

## Development

To generate the latest icons:

```bash
./bin/generate
```

Update the `VERSION` constant in `lib/sitemap.xmltool/version.rb`, then open a pull request.

Thanks! ✌️

## Roadmap

- [ ] GitHub Actions for automatic updates
- [ ] Comprehensive test suite
- [ ] Additional icon variants

## Inspiration

This project was inspired by:

- [audio-icons](https://github.com/user/audio-icons) - Great implementation reference
- [icon-library](https://github.com/user/icon-library) - Excellent architecture patterns

We thank the authors for their contributions to the ecosystem.

## Contributing

Bug reports and pull requests welcome on GitHub. This project is a safe, welcoming space for collaboration.

## License

Available as open source under the [MIT License](https://opensource.org/licenses/MIT).

## Code of Conduct

Everyone interacting in sitemap.xmltool is expected to follow the [code of conduct](CODE_OF_CONDUCT.md).

