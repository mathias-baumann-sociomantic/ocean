* `ocean.io.serialize.StringStructSerializer`

  This is only applicable to D2 builds.
  When serializing structs into strings, if the struct contains typedefs, then
  the typedef fields were in the past formatted as a sub-struct with a single
  field called 'value'. This is now fixed so that typedef fields are correctly
  resolved to their base types and formatted without the introduction of any
  nested sub-structs.