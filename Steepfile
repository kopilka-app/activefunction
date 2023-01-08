# frozen_string_literal: true

target :lib do
  signature "sig"

  check "lib"

  ignore "lib/active_function/version.rb"
  # Temporary disable type checking for this file due to:
  # lib/active_function/functions/strong_parameters.rb:94:44: [error] Unsupported splat node occurrence
  # │ Diagnostic ID: Ruby::UnsupportedSyntax
  # │
  # └             attribute.map { _1.send(method, *options.to_a) }
  #                                               ~~~~~~~~~~~~~
  ignore "lib/active_function/functions/strong_parameters.rb"

  library(
    "json",
    "forwardable"
  )
end
