# Minilib.Encoding.Base64

Defined in minilib-binary@0.5.1

BASE64 encoding and decoding

## Values

### namespace Minilib.Encoding.Base64

#### _b64_to_u8_table

Type: `Std::Array Std::U8`

[0..63] -> [0..255]

#### _filter_array

Type: `(a -> Std::Bool) -> Std::Array a -> Std::Array a`

Same as `to_iter >> filter(f) >> to_array`, but faster.

#### _u8_to_b64_table

Type: `Std::Array Std::U8`

[0..255] -> [0..63], or 0xFF if not a BASE64 char

#### base64_decode

Type: `Std::String -> Std::Array Std::U8`

Decodes a string which contains BASE64 characters to a byte array.
Characters other than BASE64 are ignored.

#### base64_encode

Type: `Std::Array Std::U8 -> Std::String`

Encodes a byte array to a BASE64 string.

## Types and aliases

## Traits and aliases

## Trait implementations