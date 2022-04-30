dataconf = configuration_data()
dataconf.set('BACKGROUNDDIR', backgrounddir)
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
  '12-Late-Night.png',
  bitday_timed
]

install_data(backgrounds, install_dir: backgrounddir)

foreach metadata : [
  'bitday.xml',
  'bitday-early.xml',
  'bitday-mid.xml',
  'bitday-late.xml'
  ]
  configure_file(
    input: metadata + '.in',
    output: metadata,
    configuration: dataconf,
    install: true,
    install_dir: metadatadir
  )
endforeach
