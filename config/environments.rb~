configure :production, :development do
    db = URI.parse(ENV['DATABASE_URL'] || 'postgres://localhost/development')
    
    ActiveRecord::Base.establish_connection(
        :adapter => db.scheme == 'postgres' ? 'postgresql' : db.scheme,
        :host => db.host,
        :username => 'andyalexnf',
        :password => 'cf-ok6617',
        :database => db.path[1..-1],
        :encoding => 'utf8'
    )
end
