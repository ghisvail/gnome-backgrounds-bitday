dataconf = configuration_data()
dataconf.set('datadir', datadir)

bitday_timed = configure_file(
  input: 'bitday-timed.xml.in',
  output: 'bitday-timed.xml',
  configuration: dataconf
)

backgrounds = [
  '01-Early-Morning.png',
  '02-Mid-Morning.png',
  '03-Late-Morning.png',
  '04-Early-Afternoon.png',
  '05-Mid-Afternoon.png',
  '06-Late-Afternoon.png',
  '07-Early-Evening.png',
  '08-Mid-Evening.png',
  '09-Late-Evening.png',
  '10-Early-Night.png',
  '11-Mid-Night.png',
  '12-Late-Night.png'
]

install_data([bitday_timed] + backgrounds, install_dir: backgrounddir)

bitday = configure_file(
  input: 'bitday.xml.in',
  output: 'bitday.xml',
  configuration: dataconf
)

install_data([bitday], install_dir: metadatadir)