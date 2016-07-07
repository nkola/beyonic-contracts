require "bundler/gem_tasks"
#require 'pacto/rake_task'
require 'pacto/server'

namespace :server do


  DEFAULTS = {
        stdout: true,
        log_file: 'pacto.log',
        strict: false,
        stub: true,
        live: false,
        generate: false,
        verbose: true,
        validate: true,
        directory: File.join(Dir.pwd, 'contracts'),
        port: 9000,
        format: :legacy,
        stenographer_log_file: File.expand_path('pacto_stenographer.log', Dir.pwd),
        strip_port: true
  }

  desc 'Run pacto server in stub, validating contracts'
  task :stub, [:port] do |task, args|
    port = args[:port] || 8081
    server_options = DEFAULTS.clone()
    server_options[:stub] = true

    Pacto::Server::HTTP.run('0.0.0.0',port,server_options)
  end
end
