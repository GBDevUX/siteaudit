# 📈 Siteaudit: Generate audit benchmark for your site 📈

Siteaudit will analize your site and generate google Page Speed and Lighthouse report.

## Installation

### **Use nodejs**

You can use `siteaudit` from your terminal using the npm package and run it as a binary

```sh
npm -g i siteaudit

siteaudit https://canellariccardo.it
```

### **Use docker**


## Runtime options

- `--output` specify the output directory (where your assets will be generated))
- `--config` specify a JSON file containing an extension to the configuration
- `--no-pagespeed` no pagespeed audit will be generated
- `--no-lighthouse` no lighthouse audit will be generated

## Configuration

If you pass to `siteaudit` an additional JSON file, it will be merged with initial config.

```sh
siteaduit https://canellariccardo.it --config ./config.json
```

Example:

```json
{
 "pagespeed": {
  "pages": [ "/", "/404" ]
 }
}
```

## Contributing

#### **Reporting bugs**

* Open a GitHub issue 

#### **Contributing with patches and bug fixes**

* Open a new GitHub pull request with the patch.
* Ensure the PR description clearly describes the problem and solution.


## Contributors

- Riccardo Canella [@thecreazy](https://github.com/thecreazy)


## License

MIT